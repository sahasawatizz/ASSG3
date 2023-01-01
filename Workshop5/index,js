const express = require('express')
const app = express()
const worker = require('./worker')

app.get('/',(req, res )=>{
  res.send('too na hee')
})

app.get('/pj', (req,res)=>{
  res.sendFile(__dirname +'/pj.html')
})

app.get('/about', (req,res)=>{
    res.send(worker.Hello())
})

app.get('/*', (req,res)=>{
  res.sendFile(__dirname +'/404.html')
})

app.listen(3000, ()=>{
  console.log("Start server at port[3000]")
})