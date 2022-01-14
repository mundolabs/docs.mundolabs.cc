# Buttons

```jsx
<Button mods="--primary --m --blue-400" leadingIcon="person">User</Button>
```

## **Attributes**

### **Modifiers**

#### **Required modifiers**

* Styles: `--primary`, `--secondary`, `--tertiary`
* Size: `--m` (medium), `--s` (small)
* Colour: `--[colour]`

{% hint style="info" %}
Colour modifiers use Bluelight colour name described [here](../foundations/colour.md#system-colours).
{% endhint %}

#### Additional modifiers

* Disabled: `--disabled`

### Linking

* App page linking: `pageLink=""`
* Webpage linking: `urlLink=""`

{% hint style="info" %}
The `pageLink` attribute will be prioritised over the `urlLink` when both are declared.&#x20;
{% endhint %}

### Icons

Button icons should be used only in circumstances that&#x20;

* Leading icon: `leadingIcon=""`
* Trailing icon: `trailingIcon=""`

{% hint style="info" %}
Trailing icons only are displayed for buttons that have a tertiary style and medium size.
{% endhint %}

### **States**

Default, Hover

****

