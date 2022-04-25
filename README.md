# LockdoorProject
TD7-ADRIEN-BODIN-CORENTIN-GROSOS

//lignes de codes prérequises (au minimum ?)
const sqlite3 = require('sqlite3');

let db = new sqlite3.Database('../modules/dataBaseDemo.db', error => { //récupération de la base de donnée
    if (error)
        throw error
})
recupGroupBDD(db).then((data) => data); //Récupération de la base de donnée

//Exemples d'utilisation des commandes db.xxx
db.run(CREATE TABLE CLIENT(nameClient VARCHAR(150), password VARCHAR(256))) //Table CLIENT
db.all("SELECT nameClient,password FROM CLIENT WHERE nameClient=?", [msg.name], (err, data) => {
db.run('INSERT INTO GROUPE(nameGroupe, statut) VALUES(?, ?)', [msg.group, statut]); //ajout ddu groupe dans la BDD
db.run('DELETE FROM EST_MEMBRE WHERE nameClient = ? AND nameGroupe = ?', [msg.from, msg.group])//supprime membre de la BDD
db.all(SELECT DISTINCT ${attribut} FROM GROUPE NATURAL JOIN CLIENT 
                        NATURAL JOIN ${relation} 
                        NATURAL JOIN EVENTS
                        NATURAL JOIN MESSAGES  
                        WHERE nameGroupe = ?, [nameGroupe], (err, data) => {
db.get('SELECT statut FROM GROUPE WHERE nameGroupe = ?', [nameGroup], (err, data)=>{
db.each('SELECT name FROM test', (error, data)=> {

/* Explication des méthodes du module db.
SELECT
.get // Récupérer la première ligne
.all // Récupérer toutes les lignes 
.each // Récupérer les lignes une par une

CREATE / INSERT / UPDATE / ...
.run
*/


POUR LE PROJET LOCKDOOR

//Pour récupération des données lors de l'inscription
const id = document.getElementById('id').value
const password = document.getElementById('pwd').value
//recuperation des valeurs des textbox
db.run('INSERT INTO USERS(pseudo, password) VALUES (?, ?)', [id, password]);

//supression par clics sur la page web ? Donc recuperation du pseudo / de l'ID == de l'identité du user à supprimer
// dans un tableau ? table.getElementById('xxx') // table.tr, table.td, etc // ?
db.run('DELETE FROM USERS WHERE pseudo = ?', [pseudo]);
