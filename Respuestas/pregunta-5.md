db.productos.aggregate([
  {
    $group: {
      _id: "$categoria",
      stockCategoria: { $sum: "$stock" }
    }
  }
])