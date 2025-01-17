# Motion Properties

Motion properties are represented by an **object** containing all the **animatable properties** of an **element**.

They are one of the two parts that compose a [**Variant**](/variants), with [**Transitions Declaration**](/transition-properties).

This object contains both **style** and **transform** properties.

Note that when interacting with both style and transform properties, you are **not forced** to specify **units** and can instead just use **numbers**.

The **default unit** of the vast majority of attributes will be **resolved** and **appended** to the value **dynamically**.

```javascript
{
    opacity: 0,
    scale: 0.6,
    y: 100
}
```

##### _An example of motion properties_ ☝️

## Style Properties

Style properties are used to **decompose** a regular `style` CSS **string** into individual **object keys**.

The typings are the same as the regular `style` property from **Vue templates**.

All the regular [**CSS Style**](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference) properties are **supported**.

Some keys are **forbidden** (`transition`, `rotate`, `scale`...) as they are now reserved for [**Transform Properties**](#transform-properties).

```javascript
{
    opacity: 0,
    marginTop: 10
}
```

##### _An example of style properties_ ☝️

## Transform Properties

Transform properties are used to **decompose** a regular `transform` CSS **string** into individual **object keys**.

All the regular [**CSS Transform**](https://developer.mozilla.org/en-US/docs/Web/CSS/transform#syntax) syntax arguments are **supported**.

As an addition, you can use `x`, `y`, `z` properties, that will be converted into `translateX`, `translateY` and `translateZ`.

```javascript
{
    x: 10,
    y: 20,
    scale: 1.2
}
```

##### _An example of transform properties_ ☝️
