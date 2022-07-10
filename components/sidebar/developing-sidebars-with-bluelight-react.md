# Developing Sidebars with Bluelight React

### `Sidebar`

```jsx
<Sidebar>
    
    <Sidebar.Title> /* Content */ </Sidebar.Title>
    
    <Sidebar.Category>
        /* Children */
    </Sidebar.Category>
    
    /* { <Sidebar.Category> } */
    
</Sidebar>
```

#### Child Restrictions

<table><thead><tr><th>Child Name</th><th data-type="select">Type</th><th>Restrictions</th></tr></thead><tbody><tr><td>Sidebar.Title</td><td></td><td>Must occur once, as the first child.</td></tr><tr><td>Sidebar.Category</td><td></td><td>Minimum of 1, immedietly following the <code>Sidebar.Title</code> subcomponent.</td></tr></tbody></table>

#### Properties

| Name | Description | Values | Default |
| ---- | ----------- | ------ | ------- |
| ``   |             | __     |         |

## Subcomponents

### `Sidebar.Title`

```jsx
<Sidebar.Title>
    // Content
</Sidebar.Title>
```

#### Content

#### Properties

| Name | Description | Values | Default |
| ---- | ----------- | ------ | ------- |
| ``   |             | __     |         |

### `Sidebar.Category`

```jsx
<Sidebar.Category>
    // Children
</Sidebar.Category>
```

#### Child Restrictions

<table><thead><tr><th>Child Name</th><th data-type="select">Type</th><th>Restrictions</th></tr></thead><tbody><tr><td><code></code><a href="developing-sidebars-with-bluelight-react.md#sidebar.item"><code>Sidebar.Item</code></a><code></code></td><td></td><td>Minimum of 1, unless the <code>Sidebar.Placeholder</code> subelement is used.</td></tr><tr><td><a href="developing-sidebars-with-bluelight-react.md#sidebar.childitem"><code>Sidebar.ChildItem</code></a><code></code></td><td></td><td>Must be accompanied by a parent <code>Sidebar.Item</code> subelement directly above.</td></tr><tr><td><code></code><a href="developing-sidebars-with-bluelight-react.md#sidebar.header"><code>Sidebar.Header</code></a><code></code></td><td></td><td>Cannot be used in the first <code>Sidebar.Category</code> subcomponent.</td></tr><tr><td><code></code><a href="developing-sidebars-with-bluelight-react.md#sidebar.placholder"><code>Sidebar.Placeholder</code></a><code></code></td><td></td><td>Cannot be used when  <code>Sidebar.Item</code> subelements appear in the <code>Sidebar.Category</code> subcomponent.</td></tr></tbody></table>

### `Sidebar.Header`

Headers are the title text for item categories. Headers should not be used for the first category, nor is required for any others.

```jsx
<Sidebar.Header>
    // Content
</Sidebar.Header>
```

#### Content

#### Properties

| Name   | Description                                         | Values              | Default |
| ------ | --------------------------------------------------- | ------------------- | ------- |
| `icon` | Specifies if the header is accompanied by an input. | _Boolean attribute_ | `False` |

### `Sidebar.Item`

```jsx
<Sidebar.Item>
    // Content
</Sidebar.Item>
```

#### Content

#### Properties

| Name       | Description                                             | Values                                 | Default        |
| ---------- | ------------------------------------------------------- | -------------------------------------- | -------------- |
| `pageLink` | Specifies the absolute route when clicked by the user.  | _String data type, beginning with_ `/` | _**Required**_ |
| `icon`     | Specifies the leading system icon.                      | _Any_ `SystemIcon` _names_             | _**Required**_ |

### `Sidebar.ChildItem`

```jsx
<Sidebar.ChildItem>
    // Content
</Sidebar.ChildItem>
```

#### Content

#### Properties

| Name       | Description                                             | Values                                 | Default        |
| ---------- | ------------------------------------------------------- | -------------------------------------- | -------------- |
| `pageLink` | Specifies the absolute route when clicked by the user.  | _String data type, beginning with_ `/` | _**Required**_ |

### `Sidebar.Placholder`

```jsx
<Sidebar.Placholder>
    // Content
</Sidebar.Placholder>
```

#### Content

#### Properties

| Name | Description | Values | Default |
| ---- | ----------- | ------ | ------- |
| ``   |             | __     |         |
