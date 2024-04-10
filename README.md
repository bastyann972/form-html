# Balise memo HTML

## Balise datetime

*exemple :* ``` <time datetime="2018-07-07">July 7</time> ```

## Balise lang

*exemple :* ```<p id="first-p" lang='de-DE' title="Première phrase">Alles klar bei dir</p>```

## Balise video & audio

*exemple :* ``` <video width="320" height="240" controls> <source src="movie.mp4" type="video/mp4"> ```

<video width="320" height="240" controls> <source src="movie.mp4" type="video/mp4">

 ``` <audio controls> <source src="myAudio.mp3" type="audio/mpeg" /> ```

 <audio controls> <source src="myAudio.mp3" type="audio/mpeg" />

## Balise tableau

 *exemple :*

 <table>
            <thead>
                <tr>
                    <th>Nombre de convives</th>
                    <th>Tarif par personnes</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td>1 à 9</td>
                    <td>120 &euro;</td>
                </tr>
                <tr>
                    <td>10 à 19</td>
                    <td>115 &euro;</td>
                </tr>
                <tr>
                    <td>19 et plus</td>
                    <td>90 &euro;</td>
                </tr>
            </tbody>
        </table>

```<table>
            <thead>
                <tr>
                    <th>Nombre de convives</th>
                    <th>Tarif par personnes</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td>1 à 9</td>
                    <td>120 &euro;</td>
                </tr>
                <tr>
                    <td>10 à 19</td>
                    <td>115 &euro;</td>
                </tr>
                <tr>
                    <td>19 et plus</td>
                    <td>90 &euro;</td>
                </tr>
            </tbody>
        </table>
```

## Balise formulaire

Tous les éléments d'un même formulaire HTML doivent être inclus dans une balise ``` <form> ```. Une même page peut accepter plusieurs formulaires HTML

*exemple :*

<label for="recherche"> Mot-clés : 
                <input type="search" name="champ_recherche" id="recherche">
            </label>
            <button>Rechercher</button>
        </form>
```
<form action="./toutes-les-tomates.html" method="get">
 <label for="recherche"> Mot-clés : <input type="search" name="champ_recherche" id="recherche"> </label> <button>Rechercher</button> </form> 
```

### Password

<form>
<div>
  <label for="username">Username:</label>
  <input type="text" id="username" name="username" />
</div>

<div>
  <label for="pass">Password (8 characters minimum):</label>
  <input type="password" id="pass" name="password" minlength="8" required />
</div>

<input type="submit" value="Sign in" />
</form>

```
<form>
<div>
  <label for="username">Username:</label>
  <input type="text" id="username" name="username" />
</div>

<div>
  <label for="pass">Password (8 characters minimum):</label>
  <input type="password" id="pass" name="password" minlength="8" required />
</div>

<input type="submit" value="Sign in" />
</form>
```

### Texte textare


<label for="biography">Raconte moi ta vie</label>
<textarea id="biography" name="biography" rows="10" cols="50">Vous pouvez écrire ici</textarea>

```
<label for="biography">Raconte moi ta vie</label>
<textarea id="biography" name="biography" rows="10" cols="50">Vous pouvez écrire ici</textarea>
```
###  Prénom

<label for="firstname">Prénom</label>
<input type="text" id="firstname" name="username">`

```
<label for="firstname">Prénom</label>
<input type="text" id="firstname" name="username">

```
### Email

<label for="email">Adresse courriel : </label>
<input type="email" id="email" name="email" placeholder="pseudo@nomdedomaine.com" required>

```

<label for="email">Adresse courriel : </label>
<input type="email" id="email" name="email" placeholder="pseudo@nomdedomaine.com" required>

```

D'autres attributs comme ```value```, ```disabled```, ```required```, ```placeholder```, ... servent à configurer nos champs

### input type checkbox

<input type="checkbox" id="green-paper" name="green">
<label for="green-paper">Vert</label>
<br>
<input type="checkbox" id="red-paper" name="red">
<label for="red-paper">Rouge</label>


```
<input type="checkbox" id="green-paper" name="green">
<label for="green-paper">Vert</label>
<br>
<input type="checkbox" id="red-paper" name="red">
<label for="red-paper">Rouge</label>

```

### input type radio

<input type="radio" name="text_size" id="size_1" value="small">
<label for="size_1">petite</label>
<br>
<input type="radio" name="text_size" id="size_2" value="normal">
<label for="size_2">normale</label>
<br>
<input type="radio" name="text_size" id="size_3" value="large">
<label for="size_3">grande</label>


```

<input type="radio" name="text_size" id="size_1" value="small">
<label for="size_1">petite</label>
<br>
<input type="radio" name="text_size" id="size_2" value="normal">
<label for="size_2">normale</label>
<br>
<input type="radio" name="text_size" id="size_3" value="large">
<label for="size_3">grande</label>

```
### balise select et la balise option

<label for="fruits">Quel est ton fruit préféré ?</label>
<select name="favorite_fruit" id="fruits">
    <option value="apple">Pomme</option>
    <option value="pear">Poire</option>
    <option value="cherry">Cerise</option>
</select>

``` 
<label for="fruits">Quel est ton fruit préféré ?</label>
<select name="favorite_fruit" id="fruits">
    <option value="apple">Pomme</option>
    <option value="pear">Poire</option>
    <option value="cherry">Cerise</option>
</select>

```
### input type file

<form method="post" enctype="multipart/form-data">
  <div>
    <label for="profile_pic">Choose file to upload</label>
    <input type="file"id="profile_pic"name="profile_pic"accept=".jpg, .jpeg, .png" />
  </div>
  <div>
    <button>Submit</button>
  </div>
</form>

```

<form method="post" enctype="multipart/form-data">
  <div>
    <label for="profile_pic">Choose file to upload</label>
    <input type="file"id="profile_pic"name="profile_pic"accept=".jpg, .jpeg, .png" />
  </div>
  <div>
    <button>Submit</button>
  </div>
</form>

```
### type color

<label for="bgcolor">Choisir la couleur de fond :</label>
<input type="color" value="#ff0000" id="bgcolor" >

```
<label for="bgcolor">Choisir la couleur de fond :</label>
<input type="color" value="#ff0000" id="bgcolor" >

```

### la balise datalist

<label for="deliveryTime">Vers quelle heure souhaitez-vous être livré ? </label>
<input type="time" list="popularHours" id="deliveryTime" />
<datalist id="popularHours">
  <option value="12:00"></option>
  <option value="13:00"></option>
  <option value="14:00"></option>
</datalist>

```

<label for="deliveryTime">Vers quelle heure souhaitez-vous être livré ? </label>
<input type="time" list="popularHours" id="deliveryTime" />
<datalist id="popularHours">
  <option value="12:00"></option>
  <option value="13:00"></option>
  <option value="14:00"></option>
</datalist>

```
<label for="hd-date">Quelle sera la date et l'heure de votre HappyDAY ?</label>
<input type="datetime-local" id="hd-date" name="hd-date">

```
     <label for="hd-date">Quelle sera la date et l'heure de votre Happy
                DAY ?</label>
            <input type="datetime-local" id="hd-date" name="hd-date">

```            

