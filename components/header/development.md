# Development

### `Header`

```jsx
<Header>
    <Header.Title> /* Content */ </Header.Title>
    /* [ <Header.Tags> ] */
</Header>
```

#### Child Restrictions

<table><thead><tr><th>Child Name</th><th data-type="select">Type</th><th>Restrictions</th></tr></thead><tbody><tr><td><code></code><a href="development.md#header.title"><code>Header.Title</code></a><code></code></td><td></td><td>Must occur once, as the first child.</td></tr><tr><td><code></code><a href="development.md#header.tags"><code>Header.Tags</code></a><code></code></td><td></td><td>Optional, but maximum of 1 occurance, following the <code>Header.Title</code>.</td></tr></tbody></table>

#### Parental Restrictions

Must be the first child within the `App.Content` subcomponent.

#### Properties

_None_

#### Modifiers

| Name      | Description                     | Values                                | Default Value  |
| --------- | ------------------------------- | ------------------------------------- | -------------- |
| Size      | Vertical height of the heading. | `isSmall` \| `isLarge`                | _**Required**_ |
| Alignment | Text alignment of the children. | `isLeft` \| `isCentered` \| `isRight` | `isLeft`       |

## Subcomponents

### `Header.Tags`

```jsx
<Header.Tags>
    <Header.Tag> /* Content */ </Header.Tag>
    /* { <Header.Tag> } */
</Header.Tags>
```

#### Child Restrictions

<table><thead><tr><th>Child Name</th><th data-type="select">Type</th><th>Restrictions</th></tr></thead><tbody><tr><td><code></code><a href="development.md#header.tag"><code>Header.Tag</code></a><code></code></td><td></td><td>Minimum of 1.</td></tr></tbody></table>

#### Properties

_None_

#### Modifiers

_None_

## Subelements

### `Header.Title`

```jsx
<Header.Title> /* Content */ </Header.Title>
```

#### Content

The title is the page's title, what would be the content of the `Titlebar.Title` subelement, with the same case.

#### Properties

#### Modifiers

### `Header.Tag`

```jsx
<Header.Tag> /* Content */ <Header.Tag>
```

#### Content

#### Properties

#### Modifiers
