# READ 12
## LOCAL STORAGE WEB APPS http://diveinto.html5doctor.com/storage.html
- cookies are maad mkkkkaaayyy. They claug servers with up to a few kb per https request causing uneaded data processing but was invented in the early days before local hosting.

- userData could store up to 64 kb data per domain back when microsoft released internet explorer
- "One vision is an acronym that you probably know already: SQL. In 2007, Google launched Gears, an open source cross-browser plugin which included an embedded database based on SQLite. This early prototype later influenced the creation of the Web SQL Database specification. Web SQL Database (formerly known as “WebDB”) provides a thin wrapper around a SQL database, allowing you to do things like this from JavaScript:

↶ actual working code in 4 browsers

openDatabase('documents', '1.0', 'Local document storage', 5*1024*1024, function (db) {
  db.changeVersion('', '1.0', function (t) {
    t.executeSql('CREATE TABLE docids (id, name)');
  }, error);
});"

There is a lot to read here. I finished the main page but I'm going to keep resourcing this until I understand it fully. The history and evolution is fascinating and hard to comprehend at this stage in my junior am coding trials