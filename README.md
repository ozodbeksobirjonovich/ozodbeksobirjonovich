<p align="center"><img src="https://user-images.githubusercontent.com/74038190/225813708-98b745f2-7d22-48cf-9150-083f1b00d6c9.gif" width="1400" height="500"></p>

<a href="https://git.io/typing-svg"><img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=50&pause=500&color=F78A13&center=true&random=false&width=1000&height=100&lines=Ozodbek Sobirjonovich" alt="Typing SVG" /></a>
<p align="center"><a href="https://git.io/typing-svg"><img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=50&pause=500&color=F78A13&center=true&random=false&width=1000&height=100&lines=Software Developer" alt="Typing SVG" /></a></p>


### **36-dars: Reactga kirish**

**Reja:**

1. **React nima?**
    - React — foydalanuvchi interfeyslarini yaratish uchun JavaScript kutubxonasi. Uning veb-ilovalardagi o‘rni va ahamiyati.
2. **React loyihasini yaratish**
    - `create-react-app` yordamida yangi React loyihasini yaratish va ishga tushirish.
3. **Komponentlar bilan tanishish**
    - Komponent tushunchasi, ularning turlari va React'dagi roli.
4. **Amaliyot: Birinchi React komponentini yaratish**
    - Oddiy "Salom, Dunyo!" komponentini yozish va brauzerda ko‘rish.

---

#### **1. React nima?**

**React** — foydalanuvchi interfeyslarini yaratish uchun ishlab chiqilgan open-source JavaScript kutubxonasi. Facebook tomonidan yaratilgan va hozirda uni keng jamoatchilik qo'llab-quvvatlaydi. React komponentlar asosida ishlaydi, bu esa kodni qayta ishlatish va loyihani boshqarishni osonlashtiradi.

**Asosiy xususiyatlari:**
- **Komponent asoslangan:** UI qismlarini mustaqil va qayta ishlatiladigan komponentlarga bo‘lish.
- **Virtual DOM:** Tez va samarali yangilanishlar uchun virtual DOM tizimi.
- **Unidirectional data flow:** Ma'lumotlar faqat bir yo‘l bo‘ylab oqadi, bu esa dastur tuzilishini soddalashtiradi.

#### **2. React loyihasini yaratish**

React loyihasini yaratish uchun eng qulay usullardan biri `create-react-app` vositasidan foydalanishdir. Bu vosita React ilovasini tez va oson yaratish uchun zarur bo‘lgan konfiguratsiyalarni avtomatik tarzda bajaradi.

**Qadamlar:**
1. **Node.js va npm o‘rnatish:**
    - React yaratish uchun Node.js va npm (Node Package Manager) kerak bo‘ladi. [Node.js](https://nodejs.org/) rasmiy saytiga kirib, o‘rnatish faylini yuklab oling va o‘rnating.
    - O‘rnatilganligini tekshirish uchun terminalga quyidagi buyruqlarni yozing:
        ```bash
        node -v
        npm -v
        ```
2. **create-react-app o‘rnatish:**
    - `create-react-app` global paket sifatida o‘rnatilmaydi, balki har bir yangi loyiha uchun ishlatiladi.
3. **Yangi React loyihasini yaratish:**
    - Terminalda quyidagi buyruqni bajarish:
        ```bash
        npx create-react-app my-first-react-app
        ```
    - Bu yerda `my-first-react-app` — loyihaning nomi. Siz uni istalgan nom bilan almashtirishingiz mumkin.
4. **Loyihani ishga tushirish:**
    - Yaratilgan loyihaga kirish va serverni ishga tushirish:
        ```bash
        cd my-first-react-app
        npm start
        ```
    - Brauzerda `http://localhost:3000` manziliga kirib, React ilovasining boshlang‘ich sahifasini ko‘rishingiz mumkin.

#### **3. Komponentlar bilan tanishish**

**Komponent** — React ilovasining asosiy qurilish bloklari. Har bir komponent mustaqil va qayta ishlatiladigan UI qismini ifodalaydi. Komponentlar ikki xil bo‘lishi mumkin:

- **Funktsional komponentlar:**
    - JavaScript funksiyalari sifatida yoziladi.
    - Oddiy, stateless komponentlar uchun mos.
    - ES6 arrow funksiyalaridan foydalanish mumkin.

    **Misol:**
    ```javascript
    function Greeting() {
        return <h1>Salom, Dunyo!</h1>;
    }

    export default Greeting;
    ```

- **Klass komponentlari:**
    - ES6 klasslari sifatida yoziladi.
    - Ichki holatni (state) saqlash va boshqarish imkonini beradi.
    - Lifecycle metodlariga ega.

    **Misol:**
    ```javascript
    import React, { Component } from 'react';

    class Greeting extends Component {
        render() {
            return <h1>Salom, Dunyo!</h1>;
        }
    }

    export default Greeting;
    ```

#### **4. Amaliyot: Birinchi React komponentini yaratish**

**Vazifa:** Oddiy "Salom, Dunyo!" komponentini yozish va brauzerda ko‘rish.

**Qadamlar:**
1. **Komponent yaratish:**
    - `src` papkasida `Greeting.js` nomli fayl yarating va quyidagi kodni yozing:
        ```javascript
        // Greeting.js
        import React from 'react';

        function Greeting() {
            return <h1>Salom, Dunyo!</h1>;
        }

        export default Greeting;
        ```
2. **Komponentni App.js ga qo‘shish:**
    - `App.js` faylini oching va uni quyidagicha o‘zgartiring:
        ```javascript
        // App.js
        import React from 'react';
        import Greeting from './Greeting';

        function App() {
            return (
                <div className="App">
                    <Greeting />
                </div>
            );
        }

        export default App;
        ```
3. **Loyihani yangilash:**
    - Brauzer avtomatik ravishda yangilanishi kerak. Siz "Salom, Dunyo!" matnini ko‘rasiz.

**Natija:**
Brauzerda quyidagi kabi sahifa ko‘rinadi:
```
Salom, Dunyo!
```

---

### **37-dars: JSX va komponentlar**

**Reja:**

1. **JSX nima?**
    - JSX sintaksisi va uning React'dagi vazifasi.
2. **Funktsional va klass komponentlari**
    - Funktsional komponentlar va ularni yaratish usullari.
3. **Klass komponentlari**
    - Klass asosidagi komponentlarni yaratish va ularning xususiyatlari.
4. **Amaliyot: Har ikki turdagi komponentlarni yaratish**

---

#### **1. JSX nima?**

**JSX (JavaScript XML)** — JavaScript va HTML sintaksisini birlashtirgan kengaytirilgan sintaksis. JSX yordamida React komponentlarida UI qismlarini oson va intuitiv tarzda yozish mumkin. Brauzer JSX'ni to‘g‘ridan-to‘g‘ri tushunmaydi, shuning uchun uni transpilyator (masalan, Babel) yordamida JavaScript'ga aylantirish kerak.

**Asosiy xususiyatlari:**
- **HTML-ga o‘xshash sintaksis:** Elementlarni yozishda HTML sintaksisidan foydalaniladi.
- **JavaScript ichida foydalanish:** JSX kodini JavaScript kodlari ichida yozish mumkin.
- **Kengaytirilgan imkoniyatlar:** JavaScript ifodalari (`{}` ichida) va dinamik kontentni qo‘llab-quvvatlaydi.

**Misol:**
```javascript
const element = <h1>Salom, Dunyo!</h1>;
```

#### **2. Funktsional va klass komponentlari**

**Funktsional komponentlar:**
- JavaScript funksiyalari sifatida yaratiladi.
- Oddiy va sodda komponentlar uchun mos.
- Holatni saqlash imkonini bermaydi (React Hooks bilan holat qo‘shish mumkin).

**Misol:**
```javascript
// FunctionalComponent.js
import React from 'react';

function FunctionalComponent() {
    return <h2>Bu funktsional komponent.</h2>;
}

export default FunctionalComponent;
```

**Klass komponentlari:**
- ES6 klasslari sifatida yaratiladi.
- Ichki holatni (state) saqlash va boshqarish imkonini beradi.
- Lifecycle metodlariga ega.

**Misol:**
```javascript
// ClassComponent.js
import React, { Component } from 'react';

class ClassComponent extends Component {
    render() {
        return <h2>Bu klass komponent.</h2>;
    }
}

export default ClassComponent;
```

#### **3. Klass komponentlari**

Klass komponentlari React'da ilg'or funksiyalarni qo‘llash uchun ishlatiladi. Ular lifecycle metodlari orqali komponentning turli bosqichlarida kod bajarishni ta'minlaydi.

**Misol:**
```javascript
// Welcome.js
import React, { Component } from 'react';

class Welcome extends Component {
    constructor(props) {
        super(props);
        this.state = { message: "Salom!" };
    }

    componentDidMount() {
        console.log("Welcome komponenti yuklandi.");
    }

    render() {
        return <h2>{this.state.message}, {this.props.name}!</h2>;
    }
}

export default Welcome;
```

**Qisqacha tushuntirish:**
- **constructor:** Komponent yaratishda chaqiriladi va boshlang‘ich holatni o‘rnatadi.
- **componentDidMount:** Komponent DOMga qo‘shilgandan keyin chaqiriladi.
- **render:** UI qismlarini qaytaradi.

#### **4. Amaliyot: Har ikki turdagi komponentlarni yaratish**

**Vazifa:** Funktsional va klass komponentlarini yaratish va ularni App.js ga qo‘shish.

**Qadamlar:**
1. **Funktsional komponent yaratish:**
    - `src` papkasida `FunctionalComponent.js` faylini yarating va quyidagicha yozing:
        ```javascript
        // FunctionalComponent.js
        import React from 'react';

        function FunctionalComponent() {
            return <h2>Bu funktsional komponent.</h2>;
        }

        export default FunctionalComponent;
        ```

2. **Klass komponent yaratish:**
    - `src` papkasida `ClassComponent.js` faylini yarating va quyidagicha yozing:
        ```javascript
        // ClassComponent.js
        import React, { Component } from 'react';

        class ClassComponent extends Component {
            render() {
                return <h2>Bu klass komponent.</h2>;
            }
        }

        export default ClassComponent;
        ```

3. **Komponentlarni App.js ga qo‘shish:**
    - `App.js` faylini oching va uni quyidagicha o‘zgartiring:
        ```javascript
        // App.js
        import React from 'react';
        import FunctionalComponent from './FunctionalComponent';
        import ClassComponent from './ClassComponent';

        function App() {
            return (
                <div className="App">
                    <FunctionalComponent />
                    <ClassComponent />
                </div>
            );
        }

        export default App;
        ```

4. **Loyihani yangilash:**
    - Brauzer avtomatik ravishda yangilanishi kerak. Siz ikki turdagi komponentlarni ko‘rasiz:
        ```
        Bu funktsional komponent.
        Bu klass komponent.
        ```

---

### **38-dars: Reactda style berish**

**Reja:**

1. **Inline stillar**
    - JSXda elementlarga to‘g‘ridan-to‘g‘ri stil berish.
2. **Tashqi CSS fayllarini ulash**
    - Komponentlarga alohida CSS fayllarini qo‘shish.
3. **CSS modullari va uslublash**
    - Modullar yordamida stil berish va uslublarni joylashtirish.
4. **Amaliyot: Komponentlarga turli uslublarni qo‘llash**

---

#### **1. Inline stillar**

**Inline stillar** — React komponentlarida to‘g‘ridan-to‘g‘ri JavaScript obyekti sifatida stil berish. Stil xususiyatlari camelCase formatida yoziladi.

**Misol:**
```javascript
// InlineStyleComponent.js
import React from 'react';

function InlineStyleComponent() {
    const headingStyle = {
        color: 'blue',
        backgroundColor: '#f1c40f',
        padding: '10px',
        borderRadius: '5px'
    };

    return <h2 style={headingStyle}>Inline Stil berilgan sarlavha.</h2>;
}

export default InlineStyleComponent;
```

**Qadamlar:**
1. **Komponent yaratish:**
    - `src` papkasida `InlineStyleComponent.js` faylini yarating va yuqoridagi kodni yozing.
2. **Komponentni App.js ga qo‘shish:**
    ```javascript
    // App.js
    import React from 'react';
    import InlineStyleComponent from './InlineStyleComponent';

    function App() {
        return (
            <div className="App">
                <InlineStyleComponent />
            </div>
        );
    }

    export default App;
    ```
3. **Natija:**
    - Brauzerda sarlavha ko‘k rangda, sariq fon bilan ko‘rinadi.

#### **2. Tashqi CSS fayllarini ulash**

React komponentlariga alohida CSS fayllarini qo‘shish orqali uslub berish mumkin. Bu usul kodni tartibli saqlashga yordam beradi.

**Misol:**
```css
/* ExternalStyle.css */
.heading {
    color: white;
    background-color: #2c3e50;
    padding: 15px;
    border-radius: 8px;
    text-align: center;
}
```

```javascript
// ExternalStyleComponent.js
import React from 'react';
import './ExternalStyle.css';

function ExternalStyleComponent() {
    return <h2 className="heading">Tashqi CSS fayli bilan stil berilgan sarlavha.</h2>;
}

export default ExternalStyleComponent;
```

**Qadamlar:**
1. **CSS faylini yaratish:**
    - `src` papkasida `ExternalStyle.css` faylini yarating va yuqoridagi CSS kodini yozing.
2. **Komponent yaratish:**
    - `ExternalStyleComponent.js` faylini yaratib, yuqoridagi JavaScript kodini yozing.
3. **Komponentni App.js ga qo‘shish:**
    ```javascript
    // App.js
    import React from 'react';
    import ExternalStyleComponent from './ExternalStyleComponent';

    function App() {
        return (
            <div className="App">
                <ExternalStyleComponent />
            </div>
        );
    }

    export default App;
    ```
4. **Natija:**
    - Sarlavha oq rangda, qora fon bilan ko‘rinadi.

#### **3. CSS modullari va uslublash**

**CSS modullari** — CSS fayllarini modullar sifatida import qilish imkonini beradi, bu esa klass nomlarining global maydonda o‘zaro to‘qnashuvini oldini oladi.

**Misol:**
```css
/* Button.module.css */
.button {
    background-color: #e74c3c;
    color: white;
    padding: 10px 20px;
    border: none;
    border-radius: 5px;
    cursor: pointer;
}

.button:hover {
    background-color: #c0392b;
}
```

```javascript
// ButtonComponent.js
import React from 'react';
import styles from './Button.module.css';

function ButtonComponent() {
    return <button className={styles.button}>Click Me</button>;
}

export default ButtonComponent;
```

**Qadamlar:**
1. **CSS modulini yaratish:**
    - `src` papkasida `Button.module.css` faylini yarating va yuqoridagi CSS kodini yozing.
2. **Komponent yaratish:**
    - `ButtonComponent.js` faylini yaratib, yuqoridagi JavaScript kodini yozing.
3. **Komponentni App.js ga qo‘shish:**
    ```javascript
    // App.js
    import React from 'react';
    import ButtonComponent from './ButtonComponent';

    function App() {
        return (
            <div className="App">
                <ButtonComponent />
            </div>
        );
    }

    export default App;
    ```
4. **Natija:**
    - Qizil tugma paydo bo‘ladi, sichqoncha ustiga olib kelganda rangi qoraga o‘zgaradi.

#### **4. Amaliyot: Komponentlarga turli uslublarni qo‘llash**

**Vazifa:** Turli uslublarni qo‘llab-quvvatlaydigan komponentlarni yaratish.

**Kod:**
```javascript
// StyledComponents.js
import React from 'react';
import './StyledComponents.css';

function StyledComponents() {
    return (
        <div>
            <h2 className="title">CSS Modul bilan sarlavha</h2>
            <p style={{ color: 'green', fontSize: '18px' }}>Inline stil bilan yozilgan matn.</p>
            <button className="styled-button">Styled Tugma</button>
        </div>
    );
}

export default StyledComponents;
```

```css
/* StyledComponents.css */
.title {
    color: #2ecc71;
    text-decoration: underline;
}

.styled-button {
    background-color: #3498db;
    color: white;
    padding: 10px 15px;
    border: none;
    border-radius: 4px;
    cursor: pointer;
}

.styled-button:hover {
    background-color: #2980b9;
}
```

```javascript
// App.js
import React from 'react';
import StyledComponents from './StyledComponents';

function App() {
    return (
        <div className="App">
            <StyledComponents />
        </div>
    );
}

export default App;
```

**Natija:**
- Yashil rangda va 18px o‘lchamli matn, yashil sarlavha va ko‘k rangli tugma ko‘rinadi.

---

### **39-dars: Props va komponentlararo aloqa**

**Reja:**

1. **Props nima?**
    - Komponentlarga ma'lumot uzatish uchun props tushunchasi.
2. **Props bilan ishlash**
    - Propslarni komponentlarga uzatish va ulardan foydalanish.
3. **Default props va propTypes**
    - Propslar uchun standart qiymatlar va ularning turlarini tekshirish.
4. **Amaliyot: Props yordamida dinamik komponent yaratish**

---

#### **1. Props nima?**

**Props (Properties)** — React komponentlariga tashqaridan uzatiladigan ma'lumotlar. Props komponentlarga moslashuvchanlik va qayta ishlatish imkonini beradi. Props o‘zgarmas (read-only) bo‘lib, faqat tashqi komponentlar tomonidan o‘zgartirilishi mumkin.

**Misol:**
```javascript
function Greeting(props) {
    return <h1>Salom, {props.name}!</h1>;
}
```

#### **2. Props bilan ishlash**

**Propslarni komponentlarga uzatish va ulardan foydalanish:**

**Misol:**
```javascript
// ParentComponent.js
import React from 'react';
import Greeting from './Greeting';

function ParentComponent() {
    return (
        <div>
            <Greeting name="Ali" />
            <Greeting name="Vali" />
            <Greeting name="Soliha" />
        </div>
    );
}

export default ParentComponent;
```

```javascript
// Greeting.js
import React from 'react';

function Greeting(props) {
    return <h1>Salom, {props.name}!</h1>;
}

export default Greeting;
```

**Natija:**
```
Salom, Ali!
Salom, Vali!
Salom, Soliha!
```

#### **3. Default props va propTypes**

**Default props** — Propslar uchun standart qiymatlarni belgilash imkonini beradi. Agar tashqi komponent propsni o‘tkazmasa, default qiymat ishlatiladi.

**Misol:**
```javascript
// Greeting.js
import React from 'react';
import PropTypes from 'prop-types';

function Greeting(props) {
    return <h1>Salom, {props.name}!</h1>;
}

Greeting.defaultProps = {
    name: "Dunyo"
};

Greeting.propTypes = {
    name: PropTypes.string
};

export default Greeting;
```

```javascript
// ParentComponent.js
import React from 'react';
import Greeting from './Greeting';

function ParentComponent() {
    return (
        <div>
            <Greeting name="Ali" />
            <Greeting />
        </div>
    );
}

export default ParentComponent;
```

**Natija:**
```
Salom, Ali!
Salom, Dunyo!
```

**Qisqacha tushuntirish:**
- **`defaultProps`:** Props uzatilmagan holatlarda ishlatiladigan standart qiymatlar.
- **`propTypes`:** Propsning turini tekshirish uchun ishlatiladi, bu esa xatoliklarni oldini olishga yordam beradi.

#### **4. Amaliyot: Props yordamida dinamik komponent yaratish**

**Vazifa:** Foydalanuvchi nomini va yoshini props orqali uzatadigan komponent yaratish.

**Kod:**
```javascript
// UserProfile.js
import React from 'react';
import PropTypes from 'prop-types';
import './UserProfile.css';

function UserProfile(props) {
    return (
        <div className="user-profile">
            <h2>{props.name}</h2>
            <p>Yosh: {props.age}</p>
        </div>
    );
}

UserProfile.defaultProps = {
    name: "NoName",
    age: 0
};

UserProfile.propTypes = {
    name: PropTypes.string,
    age: PropTypes.number
};

export default UserProfile;
```

```css
/* UserProfile.css */
.user-profile {
    border: 1px solid #ccc;
    padding: 15px;
    border-radius: 8px;
    width: 200px;
    margin: 10px auto;
    text-align: center;
    background-color: #f9f9f9;
}
```

```javascript
// App.js
import React from 'react';
import UserProfile from './UserProfile';

function App() {
    return (
        <div className="App">
            <UserProfile name="Ali" age={25} />
            <UserProfile name="Vali" age={30} />
            <UserProfile />
        </div>
    );
}

export default App;
```

**Natija:**
- Har bir foydalanuvchi profilida nom va yosh ko‘rsatiladi.
- Props uzatilmagan holatda, "NoName" va "0" ishlatiladi.

```
Ali
Yosh: 25

Vali
Yosh: 30

NoName
Yosh: 0
```

---

### **40-dars: Shartli renderlash**

**Reja:**

1. **Shartli renderlash nima?**
    - Shartlarga qarab komponentlarni ko‘rsatish yoki yashirish.
2. **`if-else` operatorlari bilan renderlash**
    - `if`, `else if`, `else` operatorlari yordamida shartli renderlash.
3. **Ternar operator va mantiqiy operatorlar**
    - Shartli renderlashning qisqartirilgan usullari.
4. **Amaliyot: Foydalanuvchi autentifikatsiyasini shartli renderlash**

---

#### **1. Shartli renderlash nima?**

**Shartli renderlash** — React komponentlarida shartlarga asoslangan holda UI qismlarini ko‘rsatish yoki yashirish usulidir. Bu foydalanuvchi interaktivligini oshirish va dinamik kontentni taqdim etish uchun ishlatiladi.

#### **2. `if-else` operatorlari bilan renderlash**

`if-else` operatorlari yordamida komponentning render funksiyasida shartlar belgilash mumkin.

**Misol:**
```javascript
// WelcomeMessage.js
import React from 'react';

function WelcomeMessage(props) {
    if (props.isLoggedIn) {
        return <h1>Salom, {props.name}!</h1>;
    } else {
        return <h1>Iltimos, tizimga kiring.</h1>;
    }
}

export default WelcomeMessage;
```

```javascript
// App.js
import React from 'react';
import WelcomeMessage from './WelcomeMessage';

function App() {
    const user = {
        name: "Ali",
        isLoggedIn: true
    };

    return (
        <div className="App">
            <WelcomeMessage name={user.name} isLoggedIn={user.isLoggedIn} />
        </div>
    );
}

export default App;
```

**Natija:**
```
Salom, Ali!
```

#### **3. Ternar operator va mantiqiy operatorlar**

**Ternar operator** — qisqa shartli ifoda yozish imkonini beradi.

**Misol:**
```javascript
// Greeting.js
import React from 'react';

function Greeting(props) {
    return (
        <h1>
            {props.isLoggedIn ? `Salom, ${props.name}!` : "Iltimos, tizimga kiring."}
        </h1>
    );
}

export default Greeting;
```

**Mantiqiy operatorlar** (`&&`) ham shartli renderlashda ishlatiladi.

**Misol:**
```javascript
// Notification.js
import React from 'react';

function Notification(props) {
    return (
        <div>
            {props.hasNotifications && <p>Sizda yangi bildirishnomalar bor!</p>}
        </div>
    );
}

export default Notification;
```

#### **4. Amaliyot: Foydalanuvchi autentifikatsiyasini shartli renderlash**

**Vazifa:** Foydalanuvchi tizimga kirganmi yoki yo‘qmi degan holatga qarab, turli komponentlarni ko‘rsatish.

**Kod:**
```javascript
// App.js
import React, { useState } from 'react';
import WelcomeMessage from './WelcomeMessage';

function App() {
    const [isLoggedIn, setIsLoggedIn] = useState(false);
    const user = {
        name: "Ali"
    };

    const toggleLogin = () => {
        setIsLoggedIn(!isLoggedIn);
    };

    return (
        <div className="App">
            <button onClick={toggleLogin}>
                {isLoggedIn ? "Tizimdan Chiqish" : "Tizimga Kirish"}
            </button>
            <WelcomeMessage name={user.name} isLoggedIn={isLoggedIn} />
        </div>
    );
}

export default App;
```

**Natija:**
- Dastlab "Iltimos, tizimga kiring." xabari ko‘rinadi.
- Tugmani bosganda, "Salom, Ali!" xabari ko‘rinadi.
- Tugma matni "Tizimga Kirish" va "Tizimdan Chiqish" o‘zgaradi.

---

### **41-dars: Ro'yxatlar va kalitlar (Keys)**

**Reja:**

1. **Ro'yxatlarni renderlash**
    - Massivlarni `map()` funksiyasi yordamida renderlash.
2. **Kalitlar (Keys) tushunchasi**
    - Kalitlarning React'dagi ahamiyati va ularni to‘g‘ri ishlatish.
3. **Elementlarni alohida komponentlarga ajratish**
    - Ro'yxat elementlarini kichik komponentlarga bo‘lish.
4. **Amaliyot: Mahsulotlar ro'yxatini dinamik ravishda ko‘rsatish**

---

#### **1. Ro'yxatlarni renderlash**

React'da massivlarni renderlash uchun `map()` funksiyasidan foydalaniladi. Har bir element uchun yangi komponent yoki JSX elementi yaratiladi.

**Misol:**
```javascript
// FruitList.js
import React from 'react';

function FruitList() {
    const fruits = ["Olma", "Banan", "Apelsin", "Uzum"];

    return (
        <ul>
            {fruits.map((fruit, index) => (
                <li key={index}>{fruit}</li>
            ))}
        </ul>
    );
}

export default FruitList;
```

**Natija:**
```
- Olma
- Banan
- Apelsin
- Uzum
```

#### **2. Kalitlar (Keys) tushunchasi**

**Kalitlar** — React ro'yxatlarda har bir elementni aniqlash uchun ishlatiladigan noyob identifikatorlar. Kalitlar React'ga qaysi elementlar o'zgarganini, qo'shilganini yoki olib tashlanganini aniqlashga yordam beradi.

**Muhim qoidalar:**
- **Uniq bo‘lishi kerak:** Har bir element uchun noyob kalit bo‘lishi zarur.
- **Barqaror bo‘lishi kerak:** Elementlar qayta tartiblanganida yoki yangilanganda kalit o'zgarmasligi kerak.
- **Indeksdan foydalanish tavsiya etilmaydi:** Elementlar dinamik ravishda qo‘shilsa yoki olib tashlansa, indekslardan foydalanish xatoliklarga olib kelishi mumkin.

**Misol:**
```javascript
// UserList.js
import React from 'react';

function UserList() {
    const users = [
        { id: 1, name: "Ali" },
        { id: 2, name: "Vali" },
        { id: 3, name: "Soliha" }
    ];

    return (
        <ul>
            {users.map(user => (
                <li key={user.id}>{user.name}</li>
            ))}
        </ul>
    );
}

export default UserList;
```

#### **3. Elementlarni alohida komponentlarga ajratish**

Ro'yxat elementlarini alohida komponentlarga bo‘lish kodni tartibli saqlash va qayta ishlatishni osonlashtiradi.

**Misol:**
```javascript
// Product.js
import React from 'react';

function Product(props) {
    return (
        <div className="product">
            <h3>{props.name}</h3>
            <p>Narxi: {props.price} $</p>
        </div>
    );
}

export default Product;
```

```javascript
// ProductList.js
import React from 'react';
import Product from './Product';

function ProductList() {
    const products = [
        { id: 1, name: "Telefon", price: 299 },
        { id: 2, name: "Kompyuter", price: 999 },
        { id: 3, name: "Planshet", price: 499 }
    ];

    return (
        <div>
            {products.map(product => (
                <Product key={product.id} name={product.name} price={product.price} />
            ))}
        </div>
    );
}

export default ProductList;
```

#### **4. Amaliyot: Mahsulotlar ro'yxatini dinamik ravishda ko‘rsatish**

**Vazifa:** Mahsulotlar ro'yxatini massivda saqlash, ularni `map()` yordamida renderlash va har bir elementga kalit berish.

**Kod:**
```javascript
// Product.js
import React from 'react';
import './Product.css';

function Product(props) {
    return (
        <div className="product">
            <h3>{props.name}</h3>
            <p>Narxi: {props.price} $</p>
        </div>
    );
}

export default Product;
```

```css
/* Product.css */
.product {
    border: 1px solid #ddd;
    padding: 15px;
    border-radius: 8px;
    margin: 10px;
    width: 200px;
    display: inline-block;
    text-align: center;
    background-color: #f9f9f9;
}
```

```javascript
// ProductList.js
import React from 'react';
import Product from './Product';

function ProductList() {
    const products = [
        { id: 1, name: "Telefon", price: 299 },
        { id: 2, name: "Kompyuter", price: 999 },
        { id: 3, name: "Planshet", price: 499 },
        { id: 4, name: "Ekran", price: 199 }
    ];

    return (
        <div>
            {products.map(product => (
                <Product key={product.id} name={product.name} price={product.price} />
            ))}
        </div>
    );
}

export default ProductList;
```

```javascript
// App.js
import React from 'react';
import ProductList from './ProductList';

function App() {
    return (
        <div className="App">
            <ProductList />
        </div>
    );
}

export default App;
```

**Natija:**
- Har bir mahsulot uchun alohida karta ko‘rinadi, unda mahsulot nomi va narxi ko‘rsatiladi.

```
Telefon
Narxi: 299 $

Kompyuter
Narxi: 999 $

Planshet
Narxi: 499 $

Ekran
Narxi: 199 $
```

---

### **42-dars: Hodisalar (Events) bilan ishlash**

**Reja:**

1. **Hodisalar nima?**
    - React'da hodisalar bilan ishlash prinsiplari.
2. **Hodisalarni qo‘llash**
    - `onClick`, `onChange`, `onSubmit` hodisalarini ishlatish.
3. **Hodisalar bilan funksiyalarni bog‘lash**
    - Hodisa yuz berganda funksiyani chaqirish usullari.
4. **Amaliyot: Tugma bosilganda holatni o‘zgartirish**

---

#### **1. Hodisalar nima?**

**Hodisalar** — foydalanuvchi interaktivligi (klik, sichqoncha harakati, klaviatura bosilishi) yoki boshqa tizim hodisalari (sahifa yuklanishi, rasm yuklanishi) natijasida yuzaga keladigan voqealar. React hodisalarini boshqarish uchun sintaksis va metodlar mavjud.

#### **2. Hodisalarni qo‘llash**

React'da hodisalarni qo‘llash uchun elementlarga hodisa atributlarini qo‘shish kerak. Hodisa atributlari camelCase formatida yoziladi.

**Misol:**
```javascript
// ClickButton.js
import React from 'react';

function ClickButton() {
    const handleClick = () => {
        alert("Tugma bosildi!");
    };

    return (
        <button onClick={handleClick}>Bosish</button>
    );
}

export default ClickButton;
```

#### **3. Hodisalar bilan funksiyalarni bog‘lash**

Hodisalar bilan funksiyalarni bog‘lashda, hodisa chaqirilganda bajarilishi kerak bo‘lgan funksiyani belgilash kerak.

**Misol:**
```javascript
// InputChange.js
import React, { useState } from 'react';

function InputChange() {
    const [value, setValue] = useState("");

    const handleChange = (event) => {
        setValue(event.target.value);
    };

    return (
        <div>
            <input type="text" value={value} onChange={handleChange} />
            <p>Kiritilgan matn: {value}</p>
        </div>
    );
}

export default InputChange;
```

#### **4. Amaliyot: Tugma bosilganda holatni o‘zgartirish**

**Vazifa:** Tugma bosilganda, komponentning holatini o‘zgartirib, matnni yangilash.

**Kod:**
```javascript
// ToggleMessage.js
import React, { useState } from 'react';

function ToggleMessage() {
    const [isVisible, setIsVisible] = useState(true);

    const toggleVisibility = () => {
        setIsVisible(!isVisible);
    };

    return (
        <div>
            <button onClick={toggleVisibility}>
                {isVisible ? "Yashirish" : "Ko‘rsatish"}
            </button>
            {isVisible && <p>Bu matn ko‘rsatilmoqda.</p>}
        </div>
    );
}

export default ToggleMessage;
```

```javascript
// App.js
import React from 'react';
import ToggleMessage from './ToggleMessage';

function App() {
    return (
        <div className="App">
            <ToggleMessage />
        </div>
    );
}

export default App;
```

**Natija:**
- Tugma bosilganda, "Bu matn ko‘rsatilmoqda." matni ko‘rinadi yoki yashiriladi.
- Tugma matni "Yashirish" va "Ko‘rsatish" o‘rtasida almashtiriladi.

---

### **43-dars: useState Hook**

**Reja:**

1. **useState nima?**
    - React'da holatni boshqarish uchun hook funksiyasi.
2. **Holatni yaratish va yangilash**
    - `const [count, setCount] = useState(0);` sintaksisi.
3. **Holat o‘zgarishiga qarab komponentni yangilash**
    - Holat o‘zgarganda avtomatik renderlash jarayoni.
4. **Amaliyot: Hisoblagich ilovasini yaratish**

---

#### **1. useState nima?**

**useState** — React Hooks'dan biri bo‘lib, funktsional komponentlarda holat (state)ni yaratish va boshqarish imkonini beradi. Hooklar React 16.8 versiyasidan boshlab qo‘llab-quvvatlanadi va klass komponentlariga alternativa sifatida ishlatiladi.

**Sintaksis:**
```javascript
const [state, setState] = useState(initialState);
```
- **state:** Holatning joriy qiymati.
- **setState:** Holatni yangilash uchun funktsiya.
- **initialState:** Holatning boshlang‘ich qiymati.

#### **2. Holatni yaratish va yangilash**

**Misol:**
```javascript
// Counter.js
import React, { useState } from 'react';

function Counter() {
    const [count, setCount] = useState(0);

    const increase = () => {
        setCount(count + 1);
    };

    const decrease = () => {
        setCount(count - 1);
    };

    return (
        <div>
            <h2>Hisoblagich: {count}</h2>
            <button onClick={increase}>+</button>
            <button onClick={decrease}>-</button>
        </div>
    );
}

export default Counter;
```

**Qisqacha tushuntirish:**
- `count` — holatning joriy qiymati.
- `setCount` — holatni yangilash funktsiyasi.
- Tugmalar bosilganda, `increase` va `decrease` funksiyalari chaqiriladi va holat yangilanadi.

#### **3. Holat o‘zgarishiga qarab komponentni yangilash**

React'da holat (state) o‘zgarganda, komponent avtomatik ravishda qayta renderlanadi va yangi holat qiymati bilan UI yangilanadi.

**Misol:**
```javascript
// ToggleText.js
import React, { useState } from 'react';

function ToggleText() {
    const [isVisible, setIsVisible] = useState(true);

    const toggle = () => {
        setIsVisible(!isVisible);
    };

    return (
        <div>
            <button onClick={toggle}>
                {isVisible ? "Yashirish" : "Ko‘rsatish"}
            </button>
            {isVisible && <p>Bu matn ko‘rsatilmoqda.</p>}
        </div>
    );
}

export default ToggleText;
```

**Natija:**
- Tugma bosilganda, "Bu matn ko‘rsatilmoqda." matni ko‘rinadi yoki yashiriladi.
- Tugma matni "Yashirish" va "Ko‘rsatish" o‘rtasida almashtiriladi.

#### **4. Amaliyot: Hisoblagich ilovasini yaratish**

**Vazifa:** Hisoblagich komponentini yaratish, uni `useState` yordamida boshqarish va tugmalar orqali hisobni oshirish yoki kamaytirish.

**Kod:**
```javascript
// Counter.js
import React, { useState } from 'react';
import './Counter.css';

function Counter() {
    const [count, setCount] = useState(0);

    const increase = () => {
        setCount(count + 1);
    };

    const decrease = () => {
        setCount(count - 1);
    };

    return (
        <div className="counter">
            <h2>Hisoblagich: {count}</h2>
            <button onClick={increase}>+</button>
            <button onClick={decrease}>-</button>
        </div>
    );
}

export default Counter;
```

```css
/* Counter.css */
.counter {
    border: 1px solid #ccc;
    padding: 20px;
    border-radius: 8px;
    width: 200px;
    margin: 20px auto;
    text-align: center;
    background-color: #f9f9f9;
}

button {
    padding: 10px 15px;
    margin: 5px;
    font-size: 18px;
    cursor: pointer;
    border: none;
    border-radius: 4px;
}

button:hover {
    background-color: #3498db;
    color: white;
}
```

```javascript
// App.js
import React from 'react';
import Counter from './Counter';

function App() {
    return (
        <div className="App">
            <Counter />
        </div>
    );
}

export default App;
```

**Natija:**
- Hisoblagichda `0` qiymati ko‘rinadi.
- "+" tugmasi bosilganda hisob 1 taga oshadi.
- "-" tugmasi bosilganda hisob 1 taga kamayadi.

---

### **44-dars: Formalar va onChange hodisasi**

**Reja:**

1. **Formalar bilan ishlash**
    - Foydalanuvchi kiritishlarini qabul qilish uchun formalar yaratish.
2. **onChange hodisasi**
    - Input qiymati o‘zgarganda hodisani tutish va holatni yangilash.
3. **Controlled komponentlar**
    - Input qiymatini holat bilan bog‘lash konsepti.
4. **Amaliyot: Ro‘yxatdan o‘tish formasini yaratish**

---

#### **1. Formalar bilan ishlash**

React'da formalar foydalanuvchi kiritishlarini qabul qilish va ularni qayta ishlash uchun ishlatiladi. Formalar input elementlari, tugmalar va boshqa interaktiv qismlardan iborat bo‘lishi mumkin.

**Misol:**
```javascript
// LoginForm.js
import React from 'react';

function LoginForm() {
    return (
        <form>
            <div>
                <label>Username:</label>
                <input type="text" name="username" />
            </div>
            <div>
                <label>Password:</label>
                <input type="password" name="password" />
            </div>
            <button type="submit">Login</button>
        </form>
    );
}

export default LoginForm;
```

#### **2. onChange hodisasi**

**onChange** hodisasi input elementida qiymat o‘zgarganda chaqiriladi. Bu hodisa orqali foydalanuvchi kiritgan ma'lumotlarni olish va holatni yangilash mumkin.

**Misol:**
```javascript
// InputHandler.js
import React, { useState } from 'react';

function InputHandler() {
    const [text, setText] = useState("");

    const handleChange = (event) => {
        setText(event.target.value);
    };

    return (
        <div>
            <input type="text" value={text} onChange={handleChange} />
            <p>Kiritilgan matn: {text}</p>
        </div>
    );
}

export default InputHandler;
```

#### **3. Controlled komponentlar**

**Controlled komponentlar** — input elementlarining qiymatini React holatiga bog‘lash konsepti. Bu usul input qiymatini holat orqali boshqarish imkonini beradi.

**Misol:**
```javascript
// ControlledInput.js
import React, { useState } from 'react';

function ControlledInput() {
    const [value, setValue] = useState("");

    const handleChange = (event) => {
        setValue(event.target.value);
    };

    return (
        <div>
            <input type="text" value={value} onChange={handleChange} />
            <p>Input qiymati: {value}</p>
        </div>
    );
}

export default ControlledInput;
```

#### **4. Amaliyot: Ro‘yxatdan o‘tish formasini yaratish**

**Vazifa:** Foydalanuvchidan ism, email va parolni qabul qiluvchi ro‘yxatdan o‘tish formasini yaratish.

**Kod:**
```javascript
// RegistrationForm.js
import React, { useState } from 'react';
import './RegistrationForm.css';

function RegistrationForm() {
    const [formData, setFormData] = useState({
        name: "",
        email: "",
        password: ""
    });

    const handleChange = (e) => {
        const { name, value } = e.target;
        setFormData(prevState => ({
            ...prevState,
            [name]: value
        }));
    };

    const handleSubmit = (e) => {
        e.preventDefault();
        console.log("Ro'yxatdan o'tgan foydalanuvchi:", formData);
        alert(`Salom, ${formData.name}! Ro'yxatdan o'tdingiz.`);
        setFormData({ name: "", email: "", password: "" });
    };

    return (
        <form onSubmit={handleSubmit} className="registration-form">
            <h2>Ro'yxatdan o'tish</h2>
            <div>
                <label>Ism:</label>
                <input
                    type="text"
                    name="name"
                    value={formData.name}
                    onChange={handleChange}
                    required
                />
            </div>
            <div>
                <label>Email:</label>
                <input
                    type="email"
                    name="email"
                    value={formData.email}
                    onChange={handleChange}
                    required
                />
            </div>
            <div>
                <label>Parol:</label>
                <input
                    type="password"
                    name="password"
                    value={formData.password}
                    onChange={handleChange}
                    required
                />
            </div>
            <button type="submit">Ro'yxatdan o'tish</button>
        </form>
    );
}

export default RegistrationForm;
```

```css
/* RegistrationForm.css */
.registration-form {
    width: 300px;
    margin: 20px auto;
    padding: 20px;
    border: 1px solid #ddd;
    border-radius: 8px;
    background-color: #f9f9f9;
}

.registration-form div {
    margin-bottom: 15px;
}

.registration-form label {
    display: block;
    margin-bottom: 5px;
}

.registration-form input {
    width: 100%;
    padding: 8px;
    box-sizing: border-box;
}

.registration-form button {
    width: 100%;
    padding: 10px;
    background-color: #2ecc71;
    color: white;
    border: none;
    border-radius: 4px;
    cursor: pointer;
}

.registration-form button:hover {
    background-color: #27ae60;
}
```

```javascript
// App.js
import React from 'react';
import RegistrationForm from './RegistrationForm';

function App() {
    return (
        <div className="App">
            <RegistrationForm />
        </div>
    );
}

export default App;
```

**Natija:**
- Foydalanuvchi ism, email va parol kiritadigan forma ko‘rinadi.
- Formani to‘ldirib yuborganidan so‘ng, foydalanuvchi ma'lumotlari konsolga chiqariladi va alert oynasi paydo bo‘ladi.
- Formani yuborishdan keyin formani tozalash amalga oshiriladi.

---

### **43-dars: Holatni yangilash va Updater funksiyalari**

**Reja:**

1. **Holatni to‘g‘ri yangilash**
    - Holatni yangilashda avvalgi holatni hisobga olish.
2. **Updater funksiyalar**
    - `setState(prevState => newState)` sintaksisidan foydalanish.
3. **Holat o‘zgarishlarining asinxronligi**
    - Holatni yangilash jarayonining asinxron xususiyati.
4. **Amaliyot: Hisoblagichni 1 sekundda bir marta oshirish**

---

#### **1. Holatni to‘g‘ri yangilash**

React'da holatni yangilashda avvalgi holatni hisobga olish zarur, ayniqsa bir nechta holat yangilanishi kerak bo‘lsa. Buning uchun `setState` funksiyasining `updater` shaklidan foydalanish tavsiya etiladi.

**Misol:**
```javascript
import React, { useState } from 'react';

function Counter() {
    const [count, setCount] = useState(0);

    const increment = () => {
        setCount(prevCount => prevCount + 1);
    };

    return (
        <div>
            <h2>Hisoblagich: {count}</h2>
            <button onClick={increment}>+</button>
        </div>
    );
}

export default Counter;
```

#### **2. Updater funksiyalar**

`setState` funksiyasining `updater` shakli, avvalgi holat qiymatini olish va yangi holat qiymatini qaytarish uchun ishlatiladi. Bu holatni yangilashda to‘g‘ri natija olishga yordam beradi, ayniqsa asinxron holat yangilanishlarida.

**Misol:**
```javascript
import React, { useState } from 'react';

function MultiIncrement() {
    const [count, setCount] = useState(0);

    const incrementTwice = () => {
        setCount(prevCount => prevCount + 1);
        setCount(prevCount => prevCount + 1);
    };

    return (
        <div>
            <h2>Hisoblagich: {count}</h2>
            <button onClick={incrementTwice}>+2</button>
        </div>
    );
}

export default MultiIncrement;
```

**Natija:**
- Tugma bosilganda hisob 2 taga oshadi.

#### **3. Holat o‘zgarishlarining asinxronligi**

React'da holatni yangilash asinxron tarzda amalga oshiriladi. Bu shuni anglatadiki, `setState` chaqirilgandan keyin holatning yangi qiymatini darhol ololmaysiz.

**Misol:**
```javascript
import React, { useState } from 'react';

function AsyncState() {
    const [count, setCount] = useState(0);

    const handleClick = () => {
        setCount(count + 1);
        console.log("Holatdan keyingi qiymat:", count); // Hali eski qiymat
    };

    return (
        <div>
            <h2>Hisoblagich: {count}</h2>
            <button onClick={handleClick}>+</button>
        </div>
    );
}

export default AsyncState;
```

**Natija:**
- Tugma bosilganda, konsolda holatdan keyingi qiymat hozircha o‘zgarmagan holda ko‘rsatiladi.

#### **4. Amaliyot: Hisoblagichni 1 sekundda bir marta oshirish**

**Vazifa:** Hisoblagichni 1 sekundda bir marta avtomatik ravishda oshiradigan komponent yaratish.

**Kod:**
```javascript
// AutoIncrement.js
import React, { useState, useEffect } from 'react';

function AutoIncrement() {
    const [count, setCount] = useState(0);

    useEffect(() => {
        const interval = setInterval(() => {
            setCount(prevCount => prevCount + 1);
        }, 1000);

        return () => clearInterval(interval);
    }, []);

    return (
        <div>
            <h2>Hisoblagich: {count}</h2>
        </div>
    );
}

export default AutoIncrement;
```

```javascript
// App.js
import React from 'react';
import AutoIncrement from './AutoIncrement';

function App() {
    return (
        <div className="App">
            <AutoIncrement />
        </div>
    );
}

export default App;
```

**Natija:**
- Hisoblagich har 1 soniyada 1 taga oshib boradi.

---

### **44-dars: Obyektlar va massivlarni holatda yangilash**

**Reja:**

1. **Holatda ob'ektlar bilan ishlash**
    - Spread operatori (`...`) yordamida ob'ektlarni yangilash.
2. **Holatda massivlarni yangilash**
    - Massivga element qo‘shish, o‘chirish va o‘zgartirish.
3. **Ob'ektlar massivini yangilash**
    - Massiv ichidagi ob'ektlarning xususiyatlarini yangilash.
4. **Amaliyot: To-Do List ilovasini yaratish**

---

#### **1. Holatda ob'ektlar bilan ishlash**

React holatida ob'ektlarni yangilashda, avvalgi holatni spread operatori yordamida saqlab, kerakli xususiyatlarni o‘zgartirish kerak.

**Misol:**
```javascript
import React, { useState } from 'react';

function UserProfile() {
    const [user, setUser] = useState({
        name: "Ali",
        age: 25,
        email: "ali@example.com"
    });

    const updateEmail = () => {
        setUser(prevUser => ({
            ...prevUser,
            email: "ali.new@example.com"
        }));
    };

    return (
        <div>
            <h2>{user.name}</h2>
            <p>Yosh: {user.age}</p>
            <p>Email: {user.email}</p>
            <button onClick={updateEmail}>Emailni Yangilash</button>
        </div>
    );
}

export default UserProfile;
```

**Natija:**
- Tugma bosilganda, email manzili yangilanadi.

#### **2. Holatda massivlarni yangilash**

React holatida massivlarga element qo‘shish, o‘chirish yoki o‘zgartirish uchun spread operatori yoki metodlardan foydalaniladi.

**Misol:**
```javascript
import React, { useState } from 'react';

function FruitList() {
    const [fruits, setFruits] = useState(["Olma", "Banan", "Apelsin"]);

    const addFruit = () => {
        setFruits([...fruits, "Uzum"]);
    };

    const removeFruit = () => {
        setFruits(fruits.slice(0, -1));
    };

    return (
        <div>
            <ul>
                {fruits.map((fruit, index) => (
                    <li key={index}>{fruit}</li>
                ))}
            </ul>
            <button onClick={addFruit}>Meva Qo‘shish</button>
            <button onClick={removeFruit}>Oxirgi Mevani O‘chirish</button>
        </div>
    );
}

export default FruitList;
```

**Natija:**
- "Meva Qo‘shish" tugmasi bosilganda, "Uzum" qo‘shiladi.
- "Oxirgi Mevani O‘chirish" tugmasi bosilganda, oxirgi meva o‘chiriladi.

#### **3. Ob'ektlar massivini yangilash**

Massiv ichidagi ob'ektlarning xususiyatlarini yangilashda, har bir ob'ektni alohida yangilash kerak.

**Misol:**
```javascript
import React, { useState } from 'react';

function ProductList() {
    const [products, setProducts] = useState([
        { id: 1, name: "Telefon", price: 299 },
        { id: 2, name: "Kompyuter", price: 999 },
        { id: 3, name: "Planshet", price: 499 }
    ]);

    const updatePrice = (id, newPrice) => {
        setProducts(products.map(product => 
            product.id === id ? { ...product, price: newPrice } : product
        ));
    };

    return (
        <div>
            {products.map(product => (
                <div key={product.id}>
                    <h3>{product.name}</h3>
                    <p>Narxi: {product.price} $</p>
                    <button onClick={() => updatePrice(product.id, product.price + 50)}>
                        Narxni Oshirish
                    </button>
                </div>
            ))}
        </div>
    );
}

export default ProductList;
```

**Natija:**
- Har bir mahsulot kartasida "Narxni Oshirish" tugmasi mavjud.
- Tugma bosilganda, mahsulot narxi 50 $ ga oshadi.

#### **4. Amaliyot: To-Do List ilovasini yaratish**

**Vazifa:** Foydalanuvchidan vazifalarni qabul qilish, ularni ro‘yxatga qo‘shish va o‘chirish imkonini beruvchi To-Do List ilovasini yaratish.

**Kod:**
```javascript
// TodoList.js
import React, { useState } from 'react';
import './TodoList.css';

function TodoList() {
    const [todos, setTodos] = useState([]);
    const [input, setInput] = useState("");

    const handleChange = (e) => {
        setInput(e.target.value);
    };

    const addTodo = (e) => {
        e.preventDefault();
        if (input.trim() === "") return;
        setTodos([...todos, { id: Date.now(), text: input }]);
        setInput("");
    };

    const removeTodo = (id) => {
        setTodos(todos.filter(todo => todo.id !== id));
    };

    return (
        <div className="todo-container">
            <h2>To-Do List</h2>
            <form onSubmit={addTodo}>
                <input
                    type="text"
                    value={input}
                    onChange={handleChange}
                    placeholder="Yangi vazifa qo‘shing..."
                />
                <button type="submit">Qo‘shish</button>
            </form>
            <ul>
                {todos.map(todo => (
                    <li key={todo.id}>
                        {todo.text}
                        <button onClick={() => removeTodo(todo.id)}>O‘chirish</button>
                    </li>
                ))}
            </ul>
        </div>
    );
}

export default TodoList;
```

```css
/* TodoList.css */
.todo-container {
    width: 400px;
    margin: 20px auto;
    padding: 20px;
    border: 1px solid #ddd;
    border-radius: 8px;
    background-color: #f9f9f9;
}

.todo-container form {
    display: flex;
    margin-bottom: 20px;
}

.todo-container input {
    flex: 1;
    padding: 10px;
    font-size: 16px;
}

.todo-container button {
    padding: 10px 15px;
    margin-left: 10px;
    font-size: 16px;
    cursor: pointer;
    border: none;
    background-color: #2ecc71;
    color: white;
    border-radius: 4px;
}

.todo-container button:hover {
    background-color: #27ae60;
}

.todo-container ul {
    list-style: none;
    padding: 0;
}

.todo-container li {
    display: flex;
    justify-content: space-between;
    padding: 8px 0;
    border-bottom: 1px solid #ccc;
}

.todo-container li button {
    background-color: #e74c3c;
    color: white;
    border: none;
    padding: 5px 10px;
    cursor: pointer;
    border-radius: 4px;
}

.todo-container li button:hover {
    background-color: #c0392b;
}
```

```javascript
// App.js
import React from 'react';
import TodoList from './TodoList';

function App() {
    return (
        <div className="App">
            <TodoList />
        </div>
    );
}

export default App;
```

**Natija:**
- Foydalanuvchi yangi vazifalarni qo‘shishi va ularni ro‘yxatdan o‘chirishi mumkin.
- Har bir vazifa ro‘yxatda ko‘rsatiladi va o‘chirish tugmasi mavjud.

---

### **45-dars: useEffect Hook**

**Reja:**

1. **useEffect nima?**
    - Yon ta'sirlarni boshqarish uchun ishlatiladigan hook.
2. **useEffect sintaksisi**
    - `useEffect(() => { /* kod */ }, [dependencies]);`
3. **Dependency array**
    - useEffect qachon ishga tushishini boshqarish uchun bog‘liqliklar ro‘yxati.
4. **Amaliyot: Vaqtni real vaqtda ko‘rsatish ilovasini yaratish**

---

#### **1. useEffect nima?**

**useEffect** — React Hooks'dan biri bo‘lib, komponentlar render qilingandan keyin bajarilishi kerak bo‘lgan yon ta'sirlarni (side effects) boshqarish uchun ishlatiladi. Yon ta'sirlar — ma'lumotlarni olish, DOMni o‘zgartirish, abonentlarni o‘rnatish va boshqalar.

#### **2. useEffect sintaksisi**

**Sintaksis:**
```javascript
useEffect(() => {
    // Kod
    return () => {
        // Tozalash kodi (optional)
    };
}, [dependencies]);
```

- **First argument:** Bajarilishi kerak bo‘lgan funksiya.
- **Second argument:** Bog‘liqliklar ro‘yxati (dependency array). Agar bu array bo‘lmasa, useEffect har renderdan keyin chaqiriladi.

**Misol:**
```javascript
import React, { useState, useEffect } from 'react';

function Timer() {
    const [seconds, setSeconds] = useState(0);

    useEffect(() => {
        const interval = setInterval(() => {
            setSeconds(prev => prev + 1);
        }, 1000);

        return () => clearInterval(interval);
    }, []);

    return (
        <div>
            <h2>Vaqt: {seconds} soniya</h2>
        </div>
    );
}

export default Timer;
```

**Qisqacha tushuntirish:**
- `useEffect` bir marta chaqiriladi (dependency array bo‘lgani uchun `[]`).
- `setInterval` orqali har 1 soniyada `seconds` holatini oshirish.
- Komponent unmount bo‘lganda, `clearInterval` chaqiriladi.

#### **3. Dependency array**

**Dependency array** — useEffect qachon chaqirilishini belgilovchi parametr. Bu array ichidagi o‘zgaruvchilar o‘zgarganida useEffect qayta chaqiriladi.

**Misol:**
```javascript
import React, { useState, useEffect } from 'react';

function CounterWithEffect() {
    const [count, setCount] = useState(0);

    useEffect(() => {
        console.log(`Hisob: ${count}`);
    }, [count]);

    return (
        <div>
            <h2>Hisob: {count}</h2>
            <button onClick={() => setCount(count + 1)}>+</button>
        </div>
    );
}

export default CounterWithEffect;
```

**Qisqacha tushuntirish:**
- `useEffect` faqat `count` o‘zgarganda chaqiriladi.
- Har bir hisob o‘sishida konsolga yangi qiymat chiqariladi.

#### **4. Amaliyot: Vaqtni real vaqtda ko‘rsatish ilovasini yaratish**

**Vazifa:** Vaqtni real vaqtda ko‘rsatadigan sekundomer (stopwatch) ilovasini yaratish.

**Kod:**
```javascript
// Stopwatch.js
import React, { useState, useEffect } from 'react';
import './Stopwatch.css';

function Stopwatch() {
    const [seconds, setSeconds] = useState(0);
    const [isActive, setIsActive] = useState(false);

    useEffect(() => {
        let interval = null;
        if (isActive) {
            interval = setInterval(() => {
                setSeconds(prevSeconds => prevSeconds + 1);
            }, 1000);
        } else if (!isActive && seconds !== 0) {
            clearInterval(interval);
        }
        return () => clearInterval(interval);
    }, [isActive, seconds]);

    const toggle = () => {
        setIsActive(!isActive);
    };

    const reset = () => {
        setSeconds(0);
        setIsActive(false);
    };

    return (
        <div className="stopwatch">
            <h2>Sekundomer</h2>
            <div className="time">
                {seconds}s
            </div>
            <button onClick={toggle}>
                {isActive ? "To‘xtatish" : "Boshlash"}
            </button>
            <button onClick={reset}>Reset</button>
        </div>
    );
}

export default Stopwatch;
```

```css
/* Stopwatch.css */
.stopwatch {
    border: 1px solid #ccc;
    padding: 20px;
    border-radius: 8px;
    width: 250px;
    margin: 20px auto;
    text-align: center;
    background-color: #f9f9f9;
}

.time {
    font-size: 48px;
    margin-bottom: 20px;
}

button {
    padding: 10px 15px;
    margin: 5px;
    font-size: 16px;
    cursor: pointer;
    border: none;
    border-radius: 4px;
}

button:hover {
    background-color: #3498db;
    color: white;
}
```

```javascript
// App.js
import React from 'react';
import Stopwatch from './Stopwatch';

function App() {
    return (
        <div className="App">
            <Stopwatch />
        </div>
    );
}

export default App;
```

**Natija:**
- Sekundomer va boshlash/to‘xtatish hamda reset tugmalari ko‘rinadi.
- "Boshlash" tugmasi bosilganda sekundomer ishga tushadi.
- "To‘xtatish" tugmasi bosilganda sekundomer to‘xtaydi.
- "Reset" tugmasi bosilganda sekundomer nolga qaytadi.

---

### **46-dars: Obyektlar va massivlarni holatda yangilash**

**Reja:**

1. **Holatda ob'ektlar bilan ishlash**
    - Spread operatori (`...`) yordamida ob'ektlarni yangilash.
2. **Holatda massivlarni yangilash**
    - Massivga element qo‘shish, o‘chirish va o‘zgartirish.
3. **Ob'ektlar massivini yangilash**
    - Massiv ichidagi ob'ektlarning xususiyatlarini yangilash.
4. **Amaliyot: To-Do List ilovasini yaratish**

---

#### **1. Holatda ob'ektlar bilan ishlash**

React'da holat ob'ektlaridan foydalanish ko‘p uchraydi. Holat ob'ektini yangilashda spread operatori (`...`) yordamida avvalgi holatni saqlash va faqat kerakli xususiyatlarni o‘zgartirish tavsiya etiladi.

**Misol:**
```javascript
import React, { useState } from 'react';

function UserProfile() {
    const [user, setUser] = useState({
        name: "Ali",
        age: 25,
        email: "ali@example.com"
    });

    const updateEmail = () => {
        setUser(prevUser => ({
            ...prevUser,
            email: "ali.new@example.com"
        }));
    };

    return (
        <div>
            <h2>{user.name}</h2>
            <p>Yosh: {user.age}</p>
            <p>Email: {user.email}</p>
            <button onClick={updateEmail}>Emailni Yangilash</button>
        </div>
    );
}

export default UserProfile;
```

**Natija:**
- "Emailni Yangilash" tugmasi bosilganda, email manzili yangilanadi.

#### **2. Holatda massivlarni yangilash**

React holatida massivlarni yangilashda ham spread operatori yoki metodlardan foydalaniladi.

**Misol:**
```javascript
import React, { useState } from 'react';

function FruitList() {
    const [fruits, setFruits] = useState(["Olma", "Banan", "Apelsin"]);

    const addFruit = () => {
        setFruits([...fruits, "Uzum"]);
    };

    const removeFruit = () => {
        setFruits(fruits.slice(0, -1));
    };

    return (
        <div>
            <ul>
                {fruits.map((fruit, index) => (
                    <li key={index}>{fruit}</li>
                ))}
            </ul>
            <button onClick={addFruit}>Meva Qo‘shish</button>
            <button onClick={removeFruit}>Oxirgi Mevani O‘chirish</button>
        </div>
    );
}

export default FruitList;
```

**Natija:**
- "Meva Qo‘shish" tugmasi bosilganda, "Uzum" qo‘shiladi.
- "Oxirgi Mevani O‘chirish" tugmasi bosilganda, oxirgi meva o‘chiriladi.

#### **3. Ob'ektlar massivini yangilash**

Massiv ichidagi ob'ektlarning xususiyatlarini yangilashda, har bir ob'ektni alohida yangilash kerak.

**Misol:**
```javascript
import React, { useState } from 'react';

function ProductList() {
    const [products, setProducts] = useState([
        { id: 1, name: "Telefon", price: 299 },
        { id: 2, name: "Kompyuter", price: 999 },
        { id: 3, name: "Planshet", price: 499 }
    ]);

    const updatePrice = (id, newPrice) => {
        setProducts(products.map(product => 
            product.id === id ? { ...product, price: newPrice } : product
        ));
    };

    return (
        <div>
            {products.map(product => (
                <div key={product.id}>
                    <h3>{product.name}</h3>
                    <p>Narxi: {product.price} $</p>
                    <button onClick={() => updatePrice(product.id, product.price + 50)}>
                        Narxni Oshirish
                    </button>
                </div>
            ))}
        </div>
    );
}

export default ProductList;
```

**Natija:**
- Har bir mahsulot kartasida "Narxni Oshirish" tugmasi mavjud.
- Tugma bosilganda, mahsulot narxi 50 $ ga oshadi.

#### **4. Amaliyot: To-Do List ilovasini yaratish**

**Vazifa:** Foydalanuvchidan vazifalarni qabul qilish, ularni ro‘yxatga qo‘shish va o‘chirish imkonini beruvchi To-Do List ilovasini yaratish.

**Kod:**
```javascript
// TodoList.js
import React, { useState } from 'react';
import './TodoList.css';

function TodoList() {
    const [todos, setTodos] = useState([]);
    const [input, setInput] = useState("");

    const handleChange = (e) => {
        setInput(e.target.value);
    };

    const addTodo = (e) => {
        e.preventDefault();
        if (input.trim() === "") return;
        setTodos([...todos, { id: Date.now(), text: input }]);
        setInput("");
    };

    const removeTodo = (id) => {
        setTodos(todos.filter(todo => todo.id !== id));
    };

    return (
        <div className="todo-container">
            <h2>To-Do List</h2>
            <form onSubmit={addTodo}>
                <input
                    type="text"
                    value={input}
                    onChange={handleChange}
                    placeholder="Yangi vazifa qo‘shing..."
                />
                <button type="submit">Qo‘shish</button>
            </form>
            <ul>
                {todos.map(todo => (
                    <li key={todo.id}>
                        {todo.text}
                        <button onClick={() => removeTodo(todo.id)}>O‘chirish</button>
                    </li>
                ))}
            </ul>
        </div>
    );
}

export default TodoList;
```

```css
/* TodoList.css */
.todo-container {
    width: 400px;
    margin: 20px auto;
    padding: 20px;
    border: 1px solid #ddd;
    border-radius: 8px;
    background-color: #f9f9f9;
}

.todo-container form {
    display: flex;
    margin-bottom: 20px;
}

.todo-container input {
    flex: 1;
    padding: 10px;
    font-size: 16px;
}

.todo-container button {
    padding: 10px 15px;
    margin-left: 10px;
    font-size: 16px;
    cursor: pointer;
    border: none;
    background-color: #2ecc71;
    color: white;
    border-radius: 4px;
}

.todo-container button:hover {
    background-color: #27ae60;
}

.todo-container ul {
    list-style: none;
    padding: 0;
}

.todo-container li {
    display: flex;
    justify-content: space-between;
    padding: 8px 0;
    border-bottom: 1px solid #ccc;
}

.todo-container li button {
    background-color: #e74c3c;
    color: white;
    border: none;
    padding: 5px 10px;
    cursor: pointer;
    border-radius: 4px;
}

.todo-container li button:hover {
    background-color: #c0392b;
}
```

```javascript
// App.js
import React from 'react';
import TodoList from './TodoList';

function App() {
    return (
        <div className="App">
            <TodoList />
        </div>
    );
}

export default App;
```

**Natija:**
- Foydalanuvchi yangi vazifalarni qo‘shishi va ularni ro‘yxatdan o‘chirishi mumkin.
- Har bir vazifa ro‘yxatda ko‘rsatiladi va o‘chirish tugmasi mavjud.

---

### **44-dars: useEffect Hook**

**Reja:**

1. **useEffect nima?**
    - Yon ta'sirlarni boshqarish uchun ishlatiladigan hook.
2. **useEffect sintaksisi**
    - `useEffect(() => { /* kod */ }, [dependencies]);`
3. **Dependency array**
    - useEffect qachon ishga tushishini boshqarish uchun bog‘liqliklar ro‘yxati.
4. **Amaliyot: Vaqtni real vaqtda ko‘rsatish ilovasini yaratish**

---

#### **1. useEffect nima?**

**useEffect** — React Hooks'dan biri bo‘lib, komponentlar render qilingandan keyin bajarilishi kerak bo‘lgan yon ta'sirlarni (side effects) boshqarish uchun ishlatiladi. Yon ta'sirlar — ma'lumotlarni olish, DOMni o‘zgartirish, abonentlarni o‘rnatish va boshqalar.

#### **2. useEffect sintaksisi**

**Sintaksis:**
```javascript
useEffect(() => {
    // Kod
    return () => {
        // Tozalash kodi (optional)
    };
}, [dependencies]);
```

- **First argument:** Bajarilishi kerak bo‘lgan funksiya.
- **Second argument:** Bog‘liqliklar ro‘yxati (dependency array). Agar bu array bo‘lmasa, useEffect har renderdan keyin chaqiriladi.

**Misol:**
```javascript
import React, { useState, useEffect } from 'react';

function Timer() {
    const [seconds, setSeconds] = useState(0);

    useEffect(() => {
        const interval = setInterval(() => {
            setSeconds(prevSeconds => prevSeconds + 1);
        }, 1000);

        return () => clearInterval(interval);
    }, []);

    return (
        <div>
            <h2>Vaqt: {seconds} soniya</h2>
        </div>
    );
}

export default Timer;
```

**Qisqacha tushuntirish:**
- `useEffect` bir marta chaqiriladi (dependency array bo‘lgani uchun `[]`).
- `setInterval` orqali har 1 soniyada `seconds` holatini oshirish.
- Komponent unmount bo‘lganda, `clearInterval` chaqiriladi.

#### **3. Dependency array**

**Dependency array** — useEffect qachon chaqirilishini belgilovchi parametr. Bu array ichidagi o‘zgaruvchilar o‘zgarganida useEffect qayta chaqiriladi.

**Misol:**
```javascript
import React, { useState, useEffect } from 'react';

function CounterWithEffect() {
    const [count, setCount] = useState(0);

    useEffect(() => {
        console.log(`Hisob: ${count}`);
    }, [count]);

    return (
        <div>
            <h2>Hisob: {count}</h2>
            <button onClick={() => setCount(count + 1)}>+</button>
        </div>
    );
}

export default CounterWithEffect;
```

**Qisqacha tushuntirish:**
- `useEffect` faqat `count` o‘zgarganda chaqiriladi.
- Har bir hisob o‘sishida konsolga yangi qiymat chiqariladi.

#### **4. Amaliyot: Vaqtni real vaqtda ko‘rsatish ilovasini yaratish**

**Vazifa:** Vaqtni real vaqtda ko‘rsatadigan sekundomer (stopwatch) ilovasini yaratish.

**Kod:**
```javascript
// Stopwatch.js
import React, { useState, useEffect } from 'react';
import './Stopwatch.css';

function Stopwatch() {
    const [seconds, setSeconds] = useState(0);
    const [isActive, setIsActive] = useState(false);

    useEffect(() => {
        let interval = null;
        if (isActive) {
            interval = setInterval(() => {
                setSeconds(prevSeconds => prevSeconds + 1);
            }, 1000);
        } else if (!isActive && seconds !== 0) {
            clearInterval(interval);
        }
        return () => clearInterval(interval);
    }, [isActive, seconds]);

    const toggle = () => {
        setIsActive(!isActive);
    };

    const reset = () => {
        setSeconds(0);
        setIsActive(false);
    };

    return (
        <div className="stopwatch">
            <h2>Sekundomer</h2>
            <div className="time">
                {seconds}s
            </div>
            <button onClick={toggle}>
                {isActive ? "To‘xtatish" : "Boshlash"}
            </button>
            <button onClick={reset}>Reset</button>
        </div>
    );
}

export default Stopwatch;
```

```css
/* Stopwatch.css */
.stopwatch {
    border: 1px solid #ccc;
    padding: 20px;
    border-radius: 8px;
    width: 250px;
    margin: 20px auto;
    text-align: center;
    background-color: #f9f9f9;
}

.time {
    font-size: 48px;
    margin-bottom: 20px;
}

button {
    padding: 10px 15px;
    margin: 5px;
    font-size: 16px;
    cursor: pointer;
    border: none;
    border-radius: 4px;
}

button:hover {
    background-color: #3498db;
    color: white;
}
```

```javascript
// App.js
import React from 'react';
import Stopwatch from './Stopwatch';

function App() {
    return (
        <div className="App">
            <Stopwatch />
        </div>
    );
}

export default App;
```

**Natija:**
- Sekundomer va boshlash/to‘xtatish hamda reset tugmalari ko‘rinadi.
- "Boshlash" tugmasi bosilganda sekundomer ishga tushadi.
- "To‘xtatish" tugmasi bosilganda sekundomer to‘xtaydi.
- "Reset" tugmasi bosilganda sekundomer nolga qaytadi.

---

### **47-dars: useContext Hook**

**Reja:**

1. **Context API nima?**
    - Komponentlar orasida ma'lumot almashish usuli.
2. **Context yaratish**
    - `React.createContext()` funksiyasi bilan context yaratish.
3. **useContext Hook**
    - Context ma'lumotlarini qulay tarzda olish uchun hook.
4. **Amaliyot: Foydalanuvchi tilini sozlash ilovasini yaratish**

---

#### **1. Context API nima?**

**Context API** — React'da komponentlar orasida ma'lumot almashish uchun ishlatiladigan tizim. U orqali chuqur joylashgan komponentlarga props orqali ma'lumot uzatmasdan to‘g‘ridan-to‘g‘ri ma'lumot yetkazish mumkin.

**Asosiy foydalanish holatlari:**
- Mavzu (theme) almashish.
- Foydalanuvchi autentifikatsiyasi.
- Til sozlamalari.

#### **2. Context yaratish**

Context yaratish uchun `React.createContext()` funksiyasidan foydalaniladi. Yaratingan context provider va consumer komponentlari mavjud bo‘ladi.

**Misol:**
```javascript
// ThemeContext.js
import React from 'react';

const ThemeContext = React.createContext('light');

export default ThemeContext;
```

#### **3. useContext Hook**

**useContext** — React Hooks'dan biri bo‘lib, context ma'lumotlarini oson va qulay tarzda olish imkonini beradi.

**Misol:**
```javascript
// ThemedButton.js
import React, { useContext } from 'react';
import ThemeContext from './ThemeContext';

function ThemedButton() {
    const theme = useContext(ThemeContext);
    const buttonStyle = {
        backgroundColor: theme === 'dark' ? '#333' : '#fff',
        color: theme === 'dark' ? '#fff' : '#333',
        padding: '10px 20px',
        border: 'none',
        borderRadius: '4px',
        cursor: 'pointer'
    };

    return <button style={buttonStyle}>Themed Button</button>;
}

export default ThemedButton;
```

```javascript
// App.js
import React, { useState } from 'react';
import ThemeContext from './ThemeContext';
import ThemedButton from './ThemedButton';

function App() {
    const [theme, setTheme] = useState('light');

    const toggleTheme = () => {
        setTheme(prevTheme => (prevTheme === 'light' ? 'dark' : 'light'));
    };

    return (
        <ThemeContext.Provider value={theme}>
            <div style={{ padding: '20px', textAlign: 'center' }}>
                <h1>useContext Hook Misoli</h1>
                <ThemedButton />
                <br /><br />
                <button onClick={toggleTheme}>
                    {theme === 'light' ? 'Dark' : 'Light'} Rejimga O‘zgartirish
                </button>
            </div>
        </ThemeContext.Provider>
    );
}

export default App;
```

**Natija:**
- "Themed Button" tugmasi hozirgi rejimga qarab rangini o‘zgartiradi.
- "Dark/Rejiming o‘zgartirish" tugmasi bosilganda, rejim almashtiriladi va tugma rangi o‘zgaradi.

#### **4. Amaliyot: Foydalanuvchi tilini sozlash ilovasini yaratish**

**Vazifa:** Foydalanuvchi tanlagan tilga qarab, sahifadagi matnlarni o‘zgartiruvchi ilova yaratish.

**Kod:**
```javascript
// LanguageContext.js
import React from 'react';

const LanguageContext = React.createContext('uz');

export default LanguageContext;
```

```javascript
// LanguageSelector.js
import React, { useContext } from 'react';
import LanguageContext from './LanguageContext';

function LanguageSelector() {
    const language = useContext(LanguageContext);

    const text = {
        uz: "Salom, dunyo!",
        en: "Hello, World!",
        ru: "Привет, мир!"
    };

    return <h2>{text[language]}</h2>;
}

export default LanguageSelector;
```

```javascript
// App.js
import React, { useState } from 'react';
import LanguageContext from './LanguageContext';
import LanguageSelector from './LanguageSelector';

function App() {
    const [language, setLanguage] = useState('uz');

    const changeLanguage = (lang) => {
        setLanguage(lang);
    };

    return (
        <LanguageContext.Provider value={language}>
            <div style={{ textAlign: 'center', marginTop: '50px' }}>
                <LanguageSelector />
                <div>
                    <button onClick={() => changeLanguage('uz')}>O'zbekcha</button>
                    <button onClick={() => changeLanguage('en')}>Inglizcha</button>
                    <button onClick={() => changeLanguage('ru')}>Ruscha</button>
                </div>
            </div>
        </LanguageContext.Provider>
    );
}

export default App;
```

**Natija:**
- Sahifada "Salom, dunyo!", "Hello, World!", yoki "Привет, мир!" matni ko‘rinadi.
- Har bir tugma bosilganda, matn tanlangan tilga qarab o‘zgaradi.

---

### **48-dars: useRef Hook va DOM bilan ishlash**

**Reja:**

1. **useRef nima?**
    - Komponentda qiymatlarni saqlash va DOM elementlariga murojaat qilish.
2. **DOM elementlariga kirish**
    - `ref` atributi yordamida elementlarni boshqarish.
3. **Holat saqlash uchun useRef**
    - Holat o‘zgarishiga olib kelmaydigan qiymatlarni saqlash.
4. **Amaliyot: Stopwatch (sekundomer) ilovasini yaratish**

---

#### **1. useRef nima?**

**useRef** — React Hooks'dan biri bo‘lib, DOM elementlariga murojaat qilish yoki komponent ichida qiymatlarni saqlash uchun ishlatiladi. useRef orqali yaratilgan ob'ektlarning `current` xususiyati orqali elementlarga yoki qiymatlarga kirish mumkin.

**Misol:**
```javascript
import React, { useRef } from 'react';

function FocusInput() {
    const inputRef = useRef(null);

    const focusInput = () => {
        inputRef.current.focus();
    };

    return (
        <div>
            <input ref={inputRef} type="text" placeholder="Foydalanuvchi kiriting" />
            <button onClick={focusInput}>Inputga Fokus</button>
        </div>
    );
}

export default FocusInput;
```

**Qisqacha tushuntirish:**
- `useRef(null)` orqali ref yaratiladi.
- `ref` atributi orqali input elementiga bog‘lanadi.
- Tugma bosilganda, inputga fokuslanadi.

#### **2. DOM elementlariga kirish**

React'da DOM elementlariga murojaat qilish uchun `useRef` ishlatiladi. Bu metod yordamida elementlarning DOM ob'ektlariga bevosita kirish mumkin.

**Misol:**
```javascript
import React, { useRef } from 'react';

function ImageToggle() {
    const imageRef = useRef(null);

    const toggleImage = () => {
        if (imageRef.current.src.includes("image1.jpg")) {
            imageRef.current.src = "image2.jpg";
        } else {
            imageRef.current.src = "image1.jpg";
        }
    };

    return (
        <div>
            <img ref={imageRef} src="image1.jpg" alt="Rasm" width="300" />
            <br />
            <button onClick={toggleImage}>Rasmni O‘zgartirish</button>
        </div>
    );
}

export default ImageToggle;
```

**Natija:**
- Tugma bosilganda, rasm `image1.jpg` va `image2.jpg` o‘rtasida almashtiriladi.

#### **3. Holat saqlash uchun useRef**

useRef orqali holat o‘zgarishiga olib kelmaydigan qiymatlarni saqlash mumkin. Bu holatlar render qilinganida saqlanib qoladi va ular o‘zgarishidan komponent qayta renderlanmaydi.

**Misol:**
```javascript
import React, { useRef } from 'react';

function Stopwatch() {
    const countRef = useRef(0);

    const increment = () => {
        countRef.current += 1;
        console.log("Hisob:", countRef.current);
    };

    return (
        <div>
            <h2>Hisob: {countRef.current}</h2>
            <button onClick={increment}>+</button>
        </div>
    );
}

export default Stopwatch;
```

**Qisqacha tushuntirish:**
- `countRef` orqali hisob saqlanadi.
- Tugma bosilganda, `countRef.current` oshiriladi va konsolga chiqariladi.
- Holat o‘zgarganiga qaramay, komponent qayta renderlanmaydi, shuning uchun ekranda hisob o‘zgarmaydi.

#### **4. Amaliyot: Stopwatch (sekundomer) ilovasini yaratish**

**Vazifa:** Sekundomer ilovasini yaratish, uning boshlash, to‘xtatish va reset qilish imkoniyatini qo‘shish.

**Kod:**
```javascript
// Stopwatch.js
import React, { useState, useEffect, useRef } from 'react';
import './Stopwatch.css';

function Stopwatch() {
    const [seconds, setSeconds] = useState(0);
    const [isActive, setIsActive] = useState(false);
    const intervalRef = useRef(null);

    useEffect(() => {
        if (isActive) {
            intervalRef.current = setInterval(() => {
                setSeconds(prevSeconds => prevSeconds + 1);
            }, 1000);
        } else if (!isActive && seconds !== 0) {
            clearInterval(intervalRef.current);
        }
        return () => clearInterval(intervalRef.current);
    }, [isActive, seconds]);

    const toggle = () => {
        setIsActive(!isActive);
    };

    const reset = () => {
        clearInterval(intervalRef.current);
        setIsActive(false);
        setSeconds(0);
    };

    return (
        <div className="stopwatch">
            <h2>Sekundomer</h2>
            <div className="time">
                {seconds}s
            </div>
            <button onClick={toggle}>
                {isActive ? "To‘xtatish" : "Boshlash"}
            </button>
            <button onClick={reset}>Reset</button>
        </div>
    );
}

export default Stopwatch;
```

```css
/* Stopwatch.css */
.stopwatch {
    border: 1px solid #ccc;
    padding: 20px;
    border-radius: 8px;
    width: 250px;
    margin: 20px auto;
    text-align: center;
    background-color: #f9f9f9;
}

.time {
    font-size: 48px;
    margin-bottom: 20px;
}

button {
    padding: 10px 15px;
    margin: 5px;
    font-size: 16px;
    cursor: pointer;
    border: none;
    border-radius: 4px;
}

button:hover {
    background-color: #3498db;
    color: white;
}
```

```javascript
// App.js
import React from 'react';
import Stopwatch from './Stopwatch';

function App() {
    return (
        <div className="App">
            <Stopwatch />
        </div>
    );
}

export default App;
```

**Natija:**
- Sekundomer va boshlash/to‘xtatish hamda reset tugmalari ko‘rinadi.
- "Boshlash" tugmasi bosilganda sekundomer ishga tushadi.
- "To‘xtatish" tugmasi bosilganda sekundomer to‘xtaydi.
- "Reset" tugmasi bosilganda sekundomer nolga qaytadi.

---

### **49-dars: useContext Hook**

**Reja:**

1. **Context API nima?**
    - Komponentlar orasida ma'lumot almashish usuli.
2. **Context yaratish**
    - `React.createContext()` funksiyasi bilan context yaratish.
3. **useContext Hook**
    - Context ma'lumotlarini qulay tarzda olish uchun hook.
4. **Amaliyot: Foydalanuvchi tilini sozlash ilovasini yaratish**

---

#### **1. Context API nima?**

**Context API** — React'da komponentlar orasida ma'lumot almashish uchun ishlatiladigan tizim. U orqali chuqur joylashgan komponentlarga props orqali ma'lumot uzatmasdan to‘g‘ridan-to‘g‘ri ma'lumot yetkazish mumkin.

**Asosiy foydalanish holatlari:**
- Mavzu (theme) almashish.
- Foydalanuvchi autentifikatsiyasi.
- Til sozlamalari.

#### **2. Context yaratish**

Context yaratish uchun `React.createContext()` funksiyasidan foydalaniladi. Yaratingan context provider va consumer komponentlari mavjud bo‘ladi.

**Misol:**
```javascript
// ThemeContext.js
import React from 'react';

const ThemeContext = React.createContext('light');

export default ThemeContext;
```

#### **3. useContext Hook**

**useContext** — React Hooks'dan biri bo‘lib, context ma'lumotlarini oson va qulay tarzda olish imkonini beradi.

**Misol:**
```javascript
// ThemedButton.js
import React, { useContext } from 'react';
import ThemeContext from './ThemeContext';

function ThemedButton() {
    const theme = useContext(ThemeContext);
    const buttonStyle = {
        backgroundColor: theme === 'dark' ? '#333' : '#fff',
        color: theme === 'dark' ? '#fff' : '#333',
        padding: '10px 20px',
        border: 'none',
        borderRadius: '4px',
        cursor: 'pointer'
    };

    return <button style={buttonStyle}>Themed Button</button>;
}

export default ThemedButton;
```

```javascript
// App.js
import React, { useState } from 'react';
import ThemeContext from './ThemeContext';
import ThemedButton from './ThemedButton';

function App() {
    const [theme, setTheme] = useState('light');

    const toggleTheme = () => {
        setTheme(prevTheme => (prevTheme === 'light' ? 'dark' : 'light'));
    };

    return (
        <ThemeContext.Provider value={theme}>
            <div style={{ padding: '20px', textAlign: 'center' }}>
                <h1>useContext Hook Misoli</h1>
                <ThemedButton />
                <br /><br />
                <button onClick={toggleTheme}>
                    {theme === 'light' ? 'Dark' : 'Light'} Rejimga O‘zgartirish
                </button>
            </div>
        </ThemeContext.Provider>
    );
}

export default App;
```

**Natija:**
- "Themed Button" tugmasi hozirgi rejimga qarab rangini o‘zgartiradi.
- "Dark/Rejiming o‘zgartirish" tugmasi bosilganda, rejim almashtiriladi va tugma rangi o‘zgaradi.

#### **4. Amaliyot: Foydalanuvchi tilini sozlash ilovasini yaratish**

**Vazifa:** Foydalanuvchi tanlagan tilga qarab, sahifadagi matnlarni o‘zgartiruvchi ilova yaratish.

**Kod:**
```javascript
// LanguageContext.js
import React from 'react';

const LanguageContext = React.createContext('uz');

export default LanguageContext;
```

```javascript
// LanguageSelector.js
import React, { useContext } from 'react';
import LanguageContext from './LanguageContext';

function LanguageSelector() {
    const language = useContext(LanguageContext);

    const text = {
        uz: "Salom, dunyo!",
        en: "Hello, World!",
        ru: "Привет, мир!"
    };

    return <h2>{text[language]}</h2>;
}

export default LanguageSelector;
```

```javascript
// App.js
import React, { useState } from 'react';
import LanguageContext from './LanguageContext';
import LanguageSelector from './LanguageSelector';

function App() {
    const [language, setLanguage] = useState('uz');

    const changeLanguage = (lang) => {
        setLanguage(lang);
    };

    return (
        <LanguageContext.Provider value={language}>
            <div style={{ textAlign: 'center', marginTop: '50px' }}>
                <LanguageSelector />
                <div>
                    <button onClick={() => changeLanguage('uz')}>O'zbekcha</button>
                    <button onClick={() => changeLanguage('en')}>Inglizcha</button>
                    <button onClick={() => changeLanguage('ru')}>Ruscha</button>
                </div>
            </div>
        </LanguageContext.Provider>
    );
}

export default App;
```

**Natija:**
- Sahifada "Salom, dunyo!", "Hello, World!", yoki "Привет, мир!" matni ko‘rinadi.
- Har bir tugma bosilganda, matn tanlangan tilga qarab o‘zgaradi.

---

### **50-dars: React ilovalarini yaratish va yakunlash**

**Reja:**

1. **Amaliyot: To‘liq React ilovasini yaratish**
    - Oldingi darslarda o‘rganilgan bilimlarni birlashtirish.
2. **Ilovani optimallashtirish**
    - Kodni refaktoring qilish, komponentlarni qayta ishlatish va yaxshilash.
3. **Kelajakdagi rivojlanish**
    - Redux, React Router va boshqa kutubxonalar bilan tanishish.
4. **Darslarni yakunlash va keyingi bosqichlar**
    - Olingan bilimlarni mustahkamlash va amaliyotda qo‘llash yo‘llari.

---

#### **1. Amaliyot: To‘liq React ilovasini yaratish**

**Vazifa:** Oldingi darslarda o‘rganilgan bilimlarni birlashtirib, to‘liq funksional React ilovasini yaratish.

**Misol: To-Do List ilovasi**

**Kod:**
```javascript
// App.js
import React from 'react';
import TodoList from './TodoList';
import Counter from './Counter';
import ToggleMessage from './ToggleMessage';
import ThemedButton from './ThemedButton';
import ThemeContext from './ThemeContext';
import './App.css';

function App() {
    return (
        <ThemeContext.Provider value="light">
            <div className="App">
                <h1>React Ilovasi</h1>
                <TodoList />
                <Counter />
                <ToggleMessage />
                <ThemedButton />
            </div>
        </ThemeContext.Provider>
    );
}

export default App;
```

```css
/* App.css */
.App {
    text-align: center;
    font-family: Arial, sans-serif;
    padding: 20px;
}
```

**Qisqacha tushuntirish:**
- Ilovada To-Do List, hisoblagich, shartli renderlash va tematik tugma komponentlari mavjud.
- `ThemeContext` orqali temani boshqarish amalga oshirilgan.

#### **2. Ilovani optimallashtirish**

Ilovani optimallashtirishda quyidagi usullarni qo‘llash mumkin:

- **Kod refaktoringi:** Kodni yanada oson o‘qiladigan va qo‘llanadigan holatga keltirish.
- **Komponentlarni qayta ishlatish:** Bir xil yoki o‘xshash UI qismlarini alohida komponentlarga bo‘lish.
- **Performance optimizatsiyasi:** `React.memo`, `useMemo`, `useCallback` kabi optimizatsiya usullarini qo‘llash.

**Misol:**
```javascript
// OptimizedProduct.js
import React from 'react';
import PropTypes from 'prop-types';
import './OptimizedProduct.css';

const OptimizedProduct = React.memo(function OptimizedProduct({ name, price }) {
    return (
        <div className="optimized-product">
            <h3>{name}</h3>
            <p>Narxi: {price} $</p>
        </div>
    );
});

OptimizedProduct.propTypes = {
    name: PropTypes.string.isRequired,
    price: PropTypes.number.isRequired
};

export default OptimizedProduct;
```

```javascript
// ProductList.js
import React from 'react';
import OptimizedProduct from './OptimizedProduct';

function ProductList({ products }) {
    return (
        <div>
            {products.map(product => (
                <OptimizedProduct key={product.id} name={product.name} price={product.price} />
            ))}
        </div>
    );
}

export default ProductList;
```

**Qisqacha tushuntirish:**
- `React.memo` yordamida komponentni memoization qilgan holda optimallashtirish.
- `PropTypes` yordamida props turlarini tekshirish.

#### **3. Kelajakdagi rivojlanish**

React ilovasini yanada rivojlantirish uchun quyidagi kutubxonalar va texnologiyalar bilan tanishish tavsiya etiladi:

- **Redux:** Keng qamrovli holat boshqarish tizimi.
- **React Router:** URL'ga asoslangan routing tizimi.
- **Styled Components:** CSS-in-JS uslubi bilan stil berish.
- **TypeScript:** React ilovasida statik tiplarni qo‘llash.
- **Next.js:** React asosidagi server-rendering ilovalari yaratish uchun freymvork.

**Misol: Redux bilan holat boshqarish:**
```javascript
// store.js
import { createStore } from 'redux';

const initialState = {
    count: 0
};

function reducer(state = initialState, action) {
    switch(action.type) {
        case 'INCREMENT':
            return { count: state.count + 1 };
        case 'DECREMENT':
            return { count: state.count - 1 };
        default:
            return state;
    }
}

const store = createStore(reducer);

export default store;
```

```javascript
// CounterWithRedux.js
import React from 'react';
import { useSelector, useDispatch } from 'react-redux';

function CounterWithRedux() {
    const count = useSelector(state => state.count);
    const dispatch = useDispatch();

    return (
        <div>
            <h2>Hisob: {count}</h2>
            <button onClick={() => dispatch({ type: 'INCREMENT' })}>+</button>
            <button onClick={() => dispatch({ type: 'DECREMENT' })}>-</button>
        </div>
    );
}

export default CounterWithRedux;
```

```javascript
// App.js
import React from 'react';
import { Provider } from 'react-redux';
import store from './store';
import CounterWithRedux from './CounterWithRedux';

function App() {
    return (
        <Provider store={store}>
            <div className="App">
                <CounterWithRedux />
            </div>
        </Provider>
    );
}

export default App;
```

**Qisqacha tushuntirish:**
- Redux orqali global holat boshqarilishi amalga oshiriladi.
- `Provider` komponenti orqali store ilovaga taqdim etiladi.
- `useSelector` va `useDispatch` yordamida holat olingan va yangilangan.

#### **4. Darslarni yakunlash va keyingi bosqichlar**

**Xulosa:**
- Bu kurs davomida React asoslarini, hooklarni, context API va boshqa asosiy funksiyalarni o‘rganib chiqdik.
- Har bir darsda amaliyotlarni bajarib, React ilovalarini yaratish bo‘yicha tajriba orttirdik.
- Keyingi bosqichlarda ilg‘or mavzular — Redux, React Router, TypeScript, va Next.js kabi texnologiyalar bilan tanishish tavsiya etiladi.

**Keyingi bosqichlar:**
- **Ilg‘or React darslari:** Hooks, render optimizatsiyasi, server-side rendering.
- **Full-Stack React:** Backend bilan integratsiya, API'lar bilan ishlash.
- **Dasturlash amaliyotlari:** Loyihalar yaratish, kod yozish mashqlari, open-source loyihalarga hissa qo‘shish.

**Maslahatlar:**
- Har doim kod yozish va amaliyotlarni bajarishda davom eting.
- React dokumentatsiyasini o‘rganib chiqing va yangi xususiyatlarni kuzatib boring.
- Kichik loyihalarni yaratib, o‘rganilgan bilimlarni mustahkamlang.

---
