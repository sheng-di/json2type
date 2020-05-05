![icon](icon.svg)

Convert json to golang, typescript, python3 type declaration.
## Usage
1. Install [tampermonkey](http://www.tampermonkey.net/).  
2. Install [this script on greasyfork](https://greasyfork.org/zh-CN/scripts/402658-jsontogo).  
2. Open browser console.  
3. In the console, following commands are supported:  

### **json text to golang type declaration**
input:
```javascript
document.jsonToGo('{"name":"user","age":18}')
```

output:
```golang
type AutoGenerated struct {
	Name string `json:"name"`
	Age int `json:"age"`
}
```

### **json text to typescript type declaration**
input:
```javascript
document.jsonToTs('{"name":"user","age":18}')
```

output:
```typescript
{
  name: string,
  age: number
}
```