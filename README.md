# react-codeflask-nextjs-typescript

```sh
yarn add react-codeflask-nextjs-typescript
```

## Usage

[Demo](https://codesandbox.io/s/cool-mountain-3n6dt)

```js
import { CodeFlaskReact } from "react-codeflask-nextjs-typescript"

class App extends React.Component {
  state = {
    code: "// enter your code"
  }

  getCodeFlaskRef = (codeFlask) => {
    this.codeFlask = codeFlask
  }

  onChange = (code) => {
    this.setState({ code })
  }

  render() {
    return (
      <CodeFlaskReact
        code={this.state.code}
        onChange={this.onChange}
        editorRef={this.getCodeFlaskRef}
      />
    )
  }
}
```
