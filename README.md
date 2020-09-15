# GameIn

## Table of Contents
- [Description](#Description)
- [Example](#Example)
- [Technologies Used](#Technologies_Used)

## Description
GameIn is a shop where you can buy a great selection of video games. The GameIn website make it easier than ever to buy the games you love.
As a GameIn member you can access new games in preview.

## Example
```javascript
authentification () {
  this.$http.get('/login', {
  })
    .then((login) => {
      if (login.data[0].username == this.email && login.data[0].password == this.password)
        {
            console.log('connecte' )
            this.currentPage='admin'
        }
        else{
          console.log('non connecte')
        }
    })

},

 addToCartr(item,index) {
    this.$http.post('/items', {
      name: this.retro[index].name,
      price: this.retro[index].price

    })
    .then(() => {
      this.items.push({
        name: this.retro[index].name,
        price: this.retro[index].price
      })
    })

}

```

## Technologies Used
- __Vue.js__ 
- __HTML5__ 
- __CSS3__ 
- __Bootstrap__ 

