# Multi-Edit

Courtesy of video - https://www.youtube.com/watch?v=p4D8-brdrZo

## Shortcuts
- `<C-b>` : Visual block mode (remapped from `<C-v>`)

### 1. Visual Block Mode (`<C-v>` or `<C-b>`)
- **Insert at Start**: Select block -> `I` -> type text -> `<Esc>` (wait a moment for it to apply to all lines).
- **Append at End**: Select block -> `$` (to end of lines) -> `A` -> type text -> `<Esc>`.
- **Change Block**: Select block -> `c` -> type text -> `<Esc>`.
- **Replace with Single Character**: Select block -> `r` -> type char.
- **Delete Block**: Select block -> `d` or `x`.

### 2. Search and Replace (Command Line)
- **Current Line**: `:s/old/new/g`
- **Entire File**: `:%s/old/new/g`
- **With Confirmation**: `:%s/old/new/gc` (y/n/a/q)
- **Visual Selection**: Select text -> `:` (will show `:'<,'>`) -> `s/old/new/g`.

## Exercises
with regex replace do the following:
 1. change const to let
 2. change (0) to (false)
 3. change useState to React.useState

```javascript
const [counter, setCounter] = useState(0);
const [count, setCount] = useState(0);
const [clicks, setClicks] = useState(0);
const [items, setItems] = useState(0);
const [data, setData] = useState(0);
const [number, setNumber] = useState(0);
const [amount, setAmount] = useState(0);
const [score, setScore] = useState(0);
const [points, setPoints] = useState(0);
const [total, setTotal] = useState(0);
const [status, setStatus] = useState(0);
const [active, setActive] = useState(0);
const [index, setIndex] = useState(0);
const [progress, setProgress] = useState(0);
const [size, setSize] = useState(0);
const [value, setValue] = useState(0);
const [state, setState] = useState(0);
const [level, setLevel] = useState(0);
const [stage, setStage] = useState(0);
const [version, setVersion] = useState(0);
```
