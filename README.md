# Entrenamiento-react



### Iteration 5 | Component: `CreditCard`

Create a `CreditCard` component that displays a rectangle with the information coming from the props. 

The component should take 8 props:

- `type`: A string that can be `"Visa"` or `"Master Card"`
- `number`: A string that is the number of the credit card. For security reasons, you should only display the 4 last digits 😉
- `expirationMonth`: A number that represents the month, between 1 and 12
- `expirationYear`: A number that represents the year
- `bank`: A string that represents the name of the bank
- `owner`: A string that represents the name of the owner
- `bgColor`: A string for the background color of the card
- `color`: A string for the text color of the card

Take your time to make the component look as close to the *expected output* as possible. You'll probably want to use flexbox.

**Example:**

```jsx
<CreditCard
  type="Visa"
  number="0123456789018845"
  expirationMonth={3}
  expirationYear={2021}
  bank="BNP"
  owner="Maxence Bouret"
  bgColor="#11aa99"
  color="white" 
/>
    
<CreditCard
  type="Master Card"
  number="0123456789010995"
  expirationMonth={3}
  expirationYear={2021}
  bank="N26"
  owner="Maxence Bouret"
  bgColor="#eeeeee"
  color="#222222"
/>
    
<CreditCard
  type="Visa"
  number="0123456789016984"
  expirationMonth={12}
  expirationYear={2019}
  bank="Name of the Bank"
  owner="Firstname Lastname"
  bgColor="#ddbb55"
  color="white" 
/>
```

**Expected Output:**

![image](https://user-images.githubusercontent.com/5306791/52975678-ac5fa000-33c6-11e9-8cbf-7d13a8a0f625.png)



----



### Iteration 6 | Component: `Rating`

Create a `Rating` component that displays 5 stars. Depending on the value received, some stars should be empty (☆), and some should be filled (★).

The component should take 1 prop:

- `children`: A number between `0` and `5`. The value can be a floating-point number. If the number received is `3.9`, the component should display 4 stars.

**Example:**

```jsx
<Rating>0</Rating>
<Rating>1.49</Rating>
<Rating>1.5</Rating>
<Rating>3</Rating>
<Rating>4</Rating>
<Rating>5</Rating>
```

**Expected Output:**

![image](https://user-images.githubusercontent.com/5306791/52972787-39512c00-33bc-11e9-93d8-428d835442fd.png)



----



### Iteration 7 | Component: `DriverCard`

Create a `DriverCard` component that displays a rectangle with content based on the received props. 

The component should take 4 props:

- `name`: A string
- `rating`: A number between `0` and `5`.  The value can be a floating point number.
- `img`: A string
- `car`: An object with properties `model` and `licensePlate`.

**Example**

```jsx
<DriverCard
  name="Travis Kalanick"
  rating={4.2}
  img="https://si.wsj.net/public/resources/images/BN-TY647_37gql_OR_20170621052140.jpg?width=620&height=428"
  car={{
    model: "Toyota Corolla Altis",
    licensePlate: "CO42DE"
  }}
/>

<DriverCard
  name="Dara Khosrowshahi"
  rating={4.9}
  img="https://ubernewsroomapi.10upcdn.com/wp-content/uploads/2017/09/Dara_ELT_Newsroom_1000px.jpg"
  car={{
    model: "Audi A3",
    licensePlate: "BE33ER"
  }}
/>
```

**Expected Output:**

![image](https://user-images.githubusercontent.com/5306791/52972847-66054380-33bc-11e9-92e0-8e48d1ab0212.png)



----



### Iteration 8 | State: `LikeButton`

Create a `LikeButton` component that displays a button with the initial text `"0 Likes"`. With each click, the number of Likes should increase.

As a bonus, implement the background color change on each click. You can use the following array of colors: `['purple','blue','green','yellow','orange','red']`

**Example:**

```jsx
<LikeButton />
```

**Expected Output:**

![](https://media.giphy.com/media/OQJkfIEkYTUdYkgNP7/giphy.gif)



----



### Iteration 9: State: `ClickablePicture`

Create a `ClickablePicture` component that displays a picture. On each click, the picture should toggle between the two images passed through the props.

**Example:**

```jsx
<ClickablePicture
  img='maxence.png'
  imgClicked='maxence-glasses.png'
/>
```

**Expected Output:**

![](https://media.giphy.com/media/9FXwCr2LLLIlgNL2sL/giphy.gif)

PS: If you want to use your picture instead, you can create it using this picture: http://www.stickpng.com/assets/images/584999937b7d4d76317f5ffd.png 😎



----



### Iteration 10 | State: `Dice`

Create a `Dice` component that displays a picture with the random dice value (example: `'../assets/images/dice3.png'`).

Every time the user clicks on the component, it should:

- First, display an empty picture (`'../assets/images/dice-empty.png'`)
- 1 second later, display a new random picture (example: `'../assets/images/dice6.png'`).

**Example:**

```jsx
<Dice />
```

**Expected Output before the click:**

![image](https://user-images.githubusercontent.com/5306791/52976705-c13e3280-33ca-11e9-8684-f4dbff643b79.png)

**Expected Output immediately after the click:**

![image](https://user-images.githubusercontent.com/5306791/52976790-25f98d00-33cb-11e9-864e-ec14b4ec2a31.png)

**Expected Output 1 second after the click:**

![image](https://user-images.githubusercontent.com/5306791/52976752-f64a8500-33ca-11e9-98ee-b0b17f5e85b2.png)



----



### Iteration 11 | State: `Carousel`

Create a `Carousel` component that displays an image and two buttons (<kbd>Left</kbd> and <kbd>Right</kbd>), which change the picture on each click, respectively.

The component should take 1 prop:

- `images`: An array of strings. Each string should be an image URL.

**Example:**

```jsx
<Carousel
  images={[
    'https://randomuser.me/api/portraits/women/1.jpg',
    'https://randomuser.me/api/portraits/men/1.jpg',
    'https://randomuser.me/api/portraits/women/2.jpg',
    'https://randomuser.me/api/portraits/men/2.jpg'
  ]}
/>
```

