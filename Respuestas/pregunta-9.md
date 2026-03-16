db.productos.aggregate([{
    $project : {nombre: 1, precio: 1, _id: 0}
}])