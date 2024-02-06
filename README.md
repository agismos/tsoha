<h1>Tenttisovellus</h1>

Sovelluksen käyttäjä on opettaja tai opiskelija. Käyttäjä voi luoda tunnuksen
joko opettajan tai opiskelijan roolissa. Jos tunnuksen luo opettajan roolissa,
tarvitaan salainen avain. Tässä vaiheessa salainen avain on abc123.

Sovellusta voi tässä vaiheessa testata paikallisesti. Kloonaamisen jälkeen
sovelluksen pitäisi käynnistyä seuraavilla komennoilla:

<ul>
  <li>python3 -m venv venv</li>
  <li>source venv/bin/activate</li>
  <li>pip install -r ./requirements.txt</li>

  <li>psql < schema.sql</li>

  <li>flask run</li>
</ul>

Mitä sovelluksessa voi tehdä tässä vaiheessa:

<ul>
  <li>Käyttäjä voi kirjautua sisään ja ulos sekä luoda uuden tunnuksen.</li>
  <li>Opiskelija näkee listan kursseista ja voi liittyä kurssille.</li>
  <li>Käyttäjä näkee yhteenvedon omista tiedoista (kesken)</li>

  <li>Opettaja pystyy luomaan uuden kurssin ja tentin.</li>

  <li>Opettaja pystyy lisäämään tenttiin kysymyksiä ja vastauksia. Vastaukset
      tallentuvat tietokantaan questions, jossa näkyy onko vastaus oikein vai väärin.</li>
</ul>

Tehtävää:
<ul>
  <li>Opiskelija voi tehdä tentin. Tätä varten täytyy luoda funktio joka hakee
      tentin kysymykset ja vastaukset tietokannasta ja luo tentin näiden perusteella. Jos kysymykseen on yksi oikea vastaus, kysymyksen muoto on avoin kysymys johon vastataan tekstikenttään. Jos kysymykseen on sekä oikeita että vääriä vastauksia, kysymys on monivalintakysymys.</li>
  <li>Opiskelija näkee yhteenvedon tekemistään tenteistä.</li>
  <li>Sovelluksen idea on olla tenttisovellus. Mutta ehkä Opettaja voi lisätä kurssille kurssimateriaalia?</li>
  <li>Opiskelija voi lähettää viestin kurssin opettajalle?</li>
  <li>Ulkoasu on alkutekijöissään. Tavoitteena tyylikäs ja yhtenäinen ilme sovellukselle.</li>
