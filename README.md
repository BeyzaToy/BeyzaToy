const siparişAlındı = new Promise(function(resolve, reject){
  if (siparişHazırlanıyor) {
    resolve('İşlem tamam!');
  } else {
    reject('Problem var...');
  }
})

siparişAlındı.then(function(cevap){
  console.log(cevap) // 'İşlem tamam!' yazısını basar
}).catch(function(hata){
  console.log(hata) // 'Problem var...' yazısını basar
})

