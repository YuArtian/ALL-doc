---
description: Provide a wide variety of icons based on react-native-vector-icons
---

# Icon

## Exemples

### Basic

![Base Usage](../.gitbook/assets/icon_base.png)

```jsx
<Icon type="antd" name="stepforward" size={30} color="#595959"/>
<Icon type="entypo" name="bug" size={30} color="#ec1f1f"/>
<Icon type="evilIcons" name="archive" size={30} color="#9c6d37"/>
<Icon type="feather" name="activity" size={30} color="#52c41a"/>
<Icon type="fontAwesome" name="500px" size={30} color="red" iconStyle={{color: '#40a9ff'}} />
<Icon type="fontAwesome5" name="amazon" style={{borderWidth: 1, borderColor: '#000', borderStyle: 'solid'}} size={30} />
<Icon type="foundation" name="heart" size={30} color="#ff68b4" />
```

### Icon Button

![Icon buttons](../.gitbook/assets/icon_buttons.png)



```jsx
<Icon.Button
  type="fontAwesome"
  name="facebook"
  backgroundColor="#3b5998"
  onPress={() => console.log('Facebook !')}>
  Facebook
</Icon.Button>
<Icon.Button
  type="fontAwesome"
  name="facebook"
  backgroundColor="#3b5998"
  iconStyle={{ color: "#ff68b4" }}
  color="#000">
  Facebook
</Icon.Button>
<Icon.Button
  type="fontAwesome"
  name="facebook"
  backgroundColor="#3b5998"
  iconStyle={{ color: "#ff68b4" }}>
  <Text style={{ fontFamily: 'Arial', fontSize: 12 }}>Facebook</Text>
</Icon.Button>
```

## API

<table>
  <thead>
    <tr>
      <th style="text-align:left">Property</th>
      <th style="text-align:left">Description</th>
      <th style="text-align:left">Type</th>
      <th style="text-align:left">Default</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left"><b><code>*name</code></b>
      </td>
      <td style="text-align:left">name of Icon , what icon to show</td>
      <td style="text-align:left"><code>string</code>
      </td>
      <td style="text-align:left"><code>-</code>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><code>type</code>
      </td>
      <td style="text-align:left">
        <p>type of bundled icon set</p>
        <p>see all icons: <a href="https://github.com/oblador/react-native-vector-icons#bundled-icon-sets">react-native-vector-icons</a>
        </p>
      </td>
      <td style="text-align:left">see all type value below</td>
      <td style="text-align:left"><code>&apos;antd&apos;</code>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><code>size</code>
      </td>
      <td style="text-align:left">size of Icon, can also be passed as <code>fontSize</code> in the style object</td>
      <td
      style="text-align:left"><code>number</code>
        </td>
        <td style="text-align:left"><code>24</code>
        </td>
    </tr>
    <tr>
      <td style="text-align:left"><code>color</code>
      </td>
      <td style="text-align:left">color of Icon</td>
      <td style="text-align:left"><code>string</code>
      </td>
      <td style="text-align:left"><code>&apos;black&apos;</code>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><code>style</code>
      </td>
      <td style="text-align:left">style of Icon Container</td>
      <td style="text-align:left"><code>View style</code>
      </td>
      <td style="text-align:left"><code>{}</code>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><code>iconStyle</code>
      </td>
      <td style="text-align:left">style of Icon only</td>
      <td style="text-align:left"><code>Text style</code>
      </td>
      <td style="text-align:left"><code>{}</code>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><code>onPress</code>
      </td>
      <td style="text-align:left">press Icon</td>
      <td style="text-align:left"><code>function</code>
      </td>
      <td style="text-align:left"><code>-</code>
      </td>
    </tr>
  </tbody>
</table>### Static Methods

<table>
  <thead>
    <tr>
      <th style="text-align:left">Method</th>
      <th style="text-align:left">Description</th>
      <th style="text-align:left">Usage</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left"><code>getFontFamily</code>
      </td>
      <td style="text-align:left">
        <p>get the fontFamily of Icon
          <br />type is required</p>
        <p>returns fontFamily name</p>
      </td>
      <td style="text-align:left"><code>Icon.getFontFamily(type)</code>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><code>hasIcon</code>
      </td>
      <td style="text-align:left">
        <p>check the name of Icon</p>
        <p>type &amp; name is required</p>
        <p>returns Boolean value true/false</p>
      </td>
      <td style="text-align:left"><code>Icon.hasIcon(type, name)</code>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><code>getRawGlyphMap</code>
      </td>
      <td style="text-align:left">
        <p>returns the raw glyph map of the icon set</p>
        <p>type is required</p>
      </td>
      <td style="text-align:left"><code>Icon.getRawGlyphMap(type)</code>
      </td>
    </tr>
  </tbody>
</table>### Icon Types

| type value | Icon |
| :--- | :--- |
| `'antd'` | [`AntDesign`](https://ant.design/) |
| `'entypo'`  | [`Entypo`](http://entypo.com/) |
| `'evilIcons'` | [`EvilIcons`](http://evil-icons.io/) |
| `'feather'` | [`Feather`](http://feathericons.com/) |
| `'fontAwesome'` | [`FontAwesome`](http://fortawesome.github.io/Font-Awesome/icons/) |
| `'fontAwesome5'` | [`FontAwesome 5`](https://fontawesome.com/) |
| `'foundation'` | [`Foundation`](http://zurb.com/playground/foundation-icon-fonts-3) |
| `'ionicons'` | [`Ionicons`](https://ionicons.com/) |
| `'materialIcons'` | [`MaterialIcons`](https://www.google.com/design/icons/) |
| `'materialCommunityIcons'` | [`MaterialCommunityIcons`](https://materialdesignicons.com/) |
| `'octicons'` | [`Octicons`](http://octicons.github.com/) |
| `'zocial'` | [`Zocial`](http://zocial.smcllns.com/) |
| `'simpleLineIcons'` | [`SimpleLineIcons`](https://simplelineicons.github.io/) |

### Icon.Button

| Property | Description | Type | Default |
| :--- | :--- | :--- | :--- |
| **`*name`** | name of Icon | `string` | `-` |
| `type` | type of Icon | `string` | `'antd'` |
| `color` | Icon and Text color | `string` | `'white'` |
| `iconStyle` | style of Icon only | `Text style` | `{marginRight: 10}` |
| `backgroundColor` | background color of button | `string` | `#007AFF` |
| `borderRadius` | border radius of button | `number` | `5` |
| `onPress` | press button | `function` | `-` |

