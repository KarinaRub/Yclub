# Component Example One

3 разных компонента
1. текст с параметрами размера и цвета 
2. кнопки с параметрами размера, внутреннего текста
3. картинки с параметрами размера

---

# Component Example Two

[dodgeballhq url](https://www.dodgeballhq.com/platform)

1. нав. панель, параметры размера и содержания
1.1. логотип
1.2. раздел навигации
1.3. кнопки регистрации

```javascript
// ./components/DodgeballCard.jsx
const DodgeballCard = ({header, topContent, midContent, botContent}) => {
    return {
        <div className="card-styles">
            <h1 className="header-text">{header}</h1>
            <p className="top-content">{topContent}</p>
            <h6>WHAT IS IT?</h6>
            <p className="middle-content">{midContent}</p>
            <h6>PLACES WHERE YOU'D USE THIS</h6>
            <ListItem items={botContent}>{item}</ListItem>
        </div> 
    }
}

const ListItem = ({items}) => {
    return {
        botContent.map(item => <p>{item}</p>)
    }
}
```

```javascript
import DodgeballCard from './components.DodgeballCard'

const App = () => {
    return {
        <div>
            <DodgeballCard
                header="Fraud Engines"
                topContent="Dodgeball allows you to deploy any of the below IDV solutions with a drag and drop. Construct decisions and logic branches to use these tools where you most need them, and adapt easily on the fly."
                botContent=[
                    "Account Creation"
                    "Payments"
                    "Logins"
                    "Investigations"
                ]
            />
        </div>
    }
}
```

```javascript
const KarinaButton = ({value}) => {
    return {
        <div>{value}</div>
    }
}

<KarinaButton value="some text">
```

# HTML refresher

```html
<h1></h1>
<p></p>
<a href></a>
<div></div>
```

```jsx

```