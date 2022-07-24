# javascript_basic
## Javascript Let আলোচনা করি 
# Destructuring কি কেন ব্যবহার করবো ?
## Object Destructuring
### single Destructuring
```
<script>

    const user = {
        name:"Al-Amin",
        roll:23,
        age:23
    }
    
    const {name:title} = user; // {name} user object name propertise amra variable change kore dite pari
    console.log(title); 

</script>

```

## Nested Destructuring

```
<script>

    const user = {
        name:"Al-Amin",
        roll:23,
        age:23,
        education:{
            degree:"Diploma"
        }
    }
    
    const {education:{degree},} = user; 
    console.log(deg); 

</script>

```
* যদি কোন কারণে education propertise না পায় তাহলে , সেই জন্য 
```
    const {education:{degree}={}} = user; 
    console.log(deg); 
 ```
 যদি education:degree না পায় তাহলে ফাকা object পাবে যার কারণে Error তা আসবে না । আমরা এভাবে useCase Error Handle করতে পারি ।
