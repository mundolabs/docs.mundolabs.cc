# Buttons

{% code title="Button.js" %}
```jsx
<button className="button --primary --red-500 --small">
    <p>
        <a>
            <Link href="/">
                <span className="material-icons">
                    trash
                </span>
                Delete
            </Link>
        </a>
    </p>
</button>
```
{% endcode %}

**MODIFIERS**

* Types:&#x20;
  * Primary: `--primary`
  * Secondary: `--secondary`
* Primary Colour: `--[COLOUR]` _(Background colour for primary type, text colour for secondary type)_
* Secondary Colour: _Automatically chosen based off background colour._&#x20;
* Size:&#x20;
  * Default: _Nothing_&#x20;
  * Small: `--small`

#### **STATES**

Default, Hover, Disabled

#### **CHILD ELEMENTS**

Leading Icon: `<span className="material-icons">[ICON]</span>`
