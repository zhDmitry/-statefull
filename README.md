# statefull
react-statefull

react statefull hoc


it add local state redux like.
```jsx
statuefull({
  title: ''
},{
  setTitle: (state, value)=> { return { ...state, title: value' }  },
  clearTitle: (state, value)=>{ return { ...state, title: '' } }
})(({ title, setTitle, clearTitle })=>{
  return <div>
  {title}
  <input onChange={e=> setTitle(e.target.value)}> title </input>
  <button onClick={clearTitle}>clear</button>
  </div>
})  
```
