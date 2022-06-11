# Buttons



## Building with Bluelight React

### **Attributes**

#### **Modifiers**

* **Styles.** `--primary`, `--secondary`, `--tertiary` — Different button styles should be used collectively to show hierarchy between actions. Button groups should only use a maximum of two different styles, either _primary/secondary_, _primary/tertiary_, or _secondary/tertiary_.
* **Size.** `--m` (medium), `--s` (small) — Button size options should be used t
* **Colour.** `--[colour]` — Colour modifiers use the Bluelight colour naming scheme described [here](../foundations/colour.md#system-colours).  Colour usage should utilise Bluelight's blanket [recommendations](../foundations/colour.md#system-colours) of using colour in user interfaces.
* **Disabled\*.** `--disabled` —

_\* — An optional modifier that is not required to be declared._

#### Linking

* **App page linking.** `pageLink=""`
* **Webpage linking.** `urlLink=""`

{% hint style="warning" %}
The `pageLink` attribute will be prioritised over the `urlLink` when both are declared, though declaring both should never be done.
{% endhint %}

#### Icons

Leading icons for buttons should be used only in circumstances that would benefit from an accompanying graphic. Consistency should be kept in mind when choosing to use or not use icons. Trailing icons should only be declared for supporting button types, and only display a chevron icon.&#x20;

* **Leading icon.** `leadingIcon=""` —&#x20;
* **Trailing icon.** `trailingIcon=""` — Trailing icons only are displayed for buttons that have a tertiary style and medium size.

### **States**

* Default, Hover



****

