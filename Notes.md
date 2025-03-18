## 3 ways to use of setup in options and composition API:

1. The traditional way in options API.
 ```vue
 <script >
    export default {
      data (){
        return{
          transactions: [
            {id:1, text:'Flowers', amount: -19.99},
            {id:2, text:'Honey', amount: -98},
            {id:3, text:'Salary', amount: 10000}
          ]
        }
      }
    }
</script>
```

2. Mixing the Compostion API.
```vue
<script >
export default {
  setup(){
    const  transactions= [
      {id:1, text:'Flowers', amount: -19.99},
      {id:2, text:'Honey', amount: -98},
      {id:3, text:'Salary', amount: 10000}
    ];

    return{
      transactions
    }
  }
}
</script>
```

3. Using pure Compostion API style.
```vue
<script setup>
  const  transactions= [
    {id:1, text:'Flowers', amount: -19.99},
    {id:2, text:'Honey', amount: -98},
    {id:3, text:'Salary', amount: 10000}
  ];
</script>
