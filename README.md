# NoSQL---MongoDB

Consultas del MongoDB:
- db.users.insertMany([ { username: 'Marjo', email: 'marjo@gmail.com', age: 23 }, { username: 'Dani', email: 'dani@gmail.com', age: 23 }, { username: 'Arantza', email: 'arantza@gmail.com', age: 33 }, { username: 'Arnold', email: 'arnold@gmail.com', age: 23 }, { username: 'Eli', email: 'eli@gmail.com', age: 26 }, { username: 'Jon', email: 'jon@gmail.com', age: 26 }, { username: 'Amaia', email: 'amaia@gmail.com', age: 27 }, { username: 'Pedro', email: 'pedro@gmail.com', age: 27 }, { username: 'Miren', email: 'miren@gmail.com', age: 27 }] )
- db.posts.insertMany([ { title: 'post1', body: 'body del post', username: 'Kepa', comments: { username: 'Kepa', body: 'comment del username' } }, { title: 'post2', body: 'body del post', username: 'Amaia', comments: { username: 'Amaia', body: 'comment del username' } }, { title: 'post3', body: 'body del post', username: 'Marjo', comments: { username: 'Marjo', body: 'comment del username' } }, { title: 'post4', body: 'body del post', username: 'Dani', comments: { username: 'Dani', body: 'comment del username' } }, { title: 'post5', body: 'body del post', username: 'Arantza', comments: { username: 'Arantza', body: 'comment del username' } }, { title: 'post6', body: 'body del post', username: 'Arnold', comments: { username: 'Arnold', body: 'comment del username' } }, { title: 'post7', body: 'body del post', username: 'Eli', comments: { username: 'Eli', body: 'comment del username' } }, { title: 'post8', body: 'body del post', username: 'Jon', comments: { username: 'Jon', body: 'comment del username' } }, { title: 'post9', body: 'body del post', username: 'Pedro', comments: { username: 'Pedro', body: 'comment del username' } }, { title: 'post10', body: 'body del post', username: 'Miren', comments: { username: 'Miren', body: 'comment del username' } }, { title: 'post11', body: 'body del post', username: 'Miren', comments: { username: 'Miren', body: 'comment del username' } }, { title: 'post12', body: 'body del post', username: 'Eli', comments: { username: 'Eli', body: 'comment del username' } }, { title: 'post13', body: 'body del post', username: 'Marjo', comments: { username: 'Marjo', body: 'comment del username' } }, { title: 'post14', body: 'body del post', username: 'Dani', comments: { username: 'Dani', body: 'comment del username' } }, { title: 'post15', body: 'body del post', username: 'Arnold', comments: { username: 'Arnold', body: 'comment del username' } }] )
- db.posts.updateOne({ title: 'post1' }, { $set: { title: 'post01', body: 'body del post 01', username: 'Arnold01', comments: { username: 'Arnold01', body: 'comment del username 01' } } })
- db.posts.updateOne( { title: 'post14' }, { $set: { comments: { username: 'Dani', body: 'comment de Dani' } } })
- db.users.updateOne({ username: 'Pedro' }, { $set: { email: 'pedropujana@gmail.com' } })
- db.users.updateOne({ username: 'Marjo' }, { $set: { email: 'marjond@gmail.com' } })
- db.users.updateOne({ username: 'Marjo' }, { $set: { age: 28 } })
- db.users.updateOne({ username: 'Miren' }, { $set: { username: 'Maria', email: 'maria@@gmail.com', age: 57 } })
- db.posts.find({ username: 'Arnold' })
- db.users.find({age:{$gt:20}})
- db.users.find({age:{$lt:23}})
- db.users.find({age:{$gte: 25, $lte: 30}})
- db.users.find().sort({ age: 1 })
- db.users.find().sort({ age: -1 })
- db.users.find()
- db.products.find()
- db.products.drop()
- db.posts.find().forEach((doc)=> { print(`Título de la publicación: ${doc.title}`) })
- db.users.find().limit(2)
- db.users.deleteOne( { age: {$gt:30} } )
- db.posts.findOne({ title: 'post13' })
- db.posts.findOne({ title: 'post15' })
## Authors

- [@kepapujana](https://www.github.com/kepapujana)

