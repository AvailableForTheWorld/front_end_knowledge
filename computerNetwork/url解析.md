### 手写url
```javascript
    function query(){
        const res = {}
        const search = location.search.substr(1);
        search.split('&').forEach(param => {
            const arr = param.split('=');
            const key = arr[0];
            const val = arr[1];
            res[key]=val;
        })
        return res;
    }
```