# Requêtes SQL de l'exercice 2.3

Si la requête est dans ce fichier, c'est qu'elle fonctionne.

|Num|Requête|
|:---:|:---|
|1| `SELECT * FROM albums;`|
|2| `SELECT * FROM albums WHERE Title LIKE '%Great%';`|
|3| `SELECT COUNT(Title) FROM albums;`|
|4| `DELETE FROM albums WHERE Title LIKE '%music%';`|
|5| `SELECT * FROM albums WHERE ArtistId='1';`|
|6| `SELECT tracks.Name, albums.Title, artists.Name FROM albums INNER JOIN artists ON albums.ArtistId=artists.ArtistId AND artists.Name='AC/DC' INNER JOIN tracks ON albums.AlbumId=tracks.AlbumId;`|
|7| `SELECT tracks.Name, albums.Title FROM tracks INNER JOIN albums ON tracks.AlbumId=albums.AlbumId AND albums.Title='Let There Be Rock';`|
|8| `SELECT SUM(tracks.UnitPrice), SUM(tracks.Milliseconds) FROM tracks INNER JOIN albums ON tracks.AlbumId=albums.AlbumId AND albums.Title='Let There Be Rock';`|
|9| `SELECT SUM(tracks.UnitPrice) FROM tracks INNER JOIN albums ON tracks.AlbumId=albums.AlbumId INNER JOIN artists ON albums.ArtistId=artists.ArtistId AND artists.Name='Deep Purple';`|
