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

<table><thead><tr><th>Child Name</th><th data-type="select">Type</th><th>Restrictions</th></tr></thead><tbody><tr><td><code></code><a href="develop.md#sidebar.title"><code>Sidebar.Title</code></a><code></code></td><td></td><td>Must occur once, as the first child.</td></tr><tr><td><a href="develop.md#sidebar.category"><code>Sidebar.Category</code></a><code></code></td><td></td><td>Minimum of 1, immedietly following the <code>Sidebar.Title</code> subcomponent.</td></tr></tbody></table>

#### Parental Restrictions

#### Properties

| Name     | Description | Values              | Default |
| -------- | ----------- | ------------------- | ------- |
| `locked` |             | _Boolean attribute_ | `True`  |

## Subcomponents

### `Sidebar.Category`

```jsx
<Sidebar.Category>
    // Children
</Sidebar.Category>
```

#### Child Restrictions

<table><thead><tr><th>Child Name</th><th data-type="select">Type</th><th>Restrictions</th></tr></thead><tbody><tr><td><code></code><a href="develop.md#sidebar.item"><code>Sidebar.Item</code></a><code></code></td><td></td><td>Minimum of 1, unless the <code>Sidebar.Placeholder</code> subelement is used.</td></tr><tr><td><a href="develop.md#sidebar.childitem"><code>Sidebar.ChildItem</code></a><code></code></td><td></td><td>Must be accompanied by a parent <code>Sidebar.Item</code> subelement directly above.</td></tr><tr><td><code></code><a href="develop.md#sidebar.header"><code>Sidebar.Header</code></a><code></code></td><td></td><td>Cannot be used in the first <code>Sidebar.Category</code> subcomponent.</td></tr><tr><td><code></code><a href="develop.md#sidebar.placholder"><code>Sidebar.Placeholder</code></a><code></code></td><td></td><td>Cannot be used when  <code>Sidebar.Item</code> subelements appear in the <code>Sidebar.Category</code> subcomponent.</td></tr></tbody></table>

#### Parental Restrictions

## Subelements

### `Sidebar.Title`

```jsx
<Sidebar.Title>
    // Content
</Sidebar.Title>
```

#### Content

The content of the `Sidebar.Title` subelement is the name of the app. This should not change between different pages in the app. The text should be in title-case.

#### Parental Restrictions

#### Properties

| Name | Description | Values | Default |
| ---- | ----------- | ------ | ------- |
| ``   |             | __     |         |

### `Sidebar.Header`

Headers are the title text for item categories. Headers should not be used for the first category, nor is required for any others.

```jsx
<Sidebar.Header>
    // Content
</Sidebar.Header>
```

#### Content

Name of pages category. Use:

* Title-case (which is then transformed by CSS to upper-case when rendering)
* First-person possession (e.g. '_My Courses'_, opposed to '_Your Courses', 'Jack's Courses',_ or just '_Courses' when possessive_)
* No sentence punctuation (no full-stops or commas)

#### Parental Restrictions

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

#### Content2

#### Parental Restrictions

#### Properties

| Name       | Description                                             | Values                                      | Default        |
| ---------- | ------------------------------------------------------- | ------------------------------------------- | -------------- |
| `pageLink` | Specifies the absolute route when clicked by the user.  | _String data type, beginning with root_ `/` | _**Required**_ |
| `icon`     | Specifies the leading system icon.                      | _Any_ `SystemIcon` _names_                  | _**Required**_ |

### `Sidebar.ChildItem`

```jsx
<Sidebar.ChildItem>
    // Content
</Sidebar.ChildItem>
```

#### Content

See [Sidebar.Item/Content](develop.md#content-2).

#### Parental Restrictions

#### Properties

| Name       | Description                                             | Values                                      | Default        |
| ---------- | ------------------------------------------------------- | ------------------------------------------- | -------------- |
| `pageLink` | Specifies the absolute route when clicked by the user.  | _String data type, beginning with root_ `/` | _**Required**_ |

### `Sidebar.Placholder`

```jsx
<Sidebar.Placholder>
    // Content
</Sidebar.Placholder>
```

#### Content

#### Parental Restrictions

#### Properties

| Name | Description | Values | Default |
| ---- | ----------- | ------ | ------- |
| ``   |             | __     |         |
