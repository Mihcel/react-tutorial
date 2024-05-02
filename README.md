# react-tutorial

Voraussetzungen:
Node.js https://nodejs.org/en/download

Neues React Projekt beginnen:
> npm create vite@latest
- React auswählen
- JavaScript auswählen
> cd [project name]

> npm install

> npm run dev

Nach Neustart von vs code Server starten:
> cd [project name]

> npm run dev


# neue React Komponente erstellen

Im src Ordner neue Datei erstellen:
> ComponentName.jsx

Die Datei muss mit Großbuchstaben beginnen und mit .jsx enden.


> function ComponentName() {
> 
>  return (
> 
>    <>
> 
>      <div>HTML Element 1</div>
> 
>      <div>HTML Element 2</div>
> 
>    </>
> 
>  );
> 
> export default ComponentName;

Es darf standardmäßig nur ein HTML Element im return statement stehen. 
Das kann umgangen werden, indem mehrere HTML Elemente in einem JSX Fragment (<> </>) eingebettet sind.


Die neu erstellte Komponente muss noch in App.jsx eingebunden werden:

> import ComponentName from "./ComponentName.jsx";
>
> function App() {
>
>   return(
>
>    <ComponentName />;
>
>   )
> 
> }
>
> export default App;

Beim Speichern der Datei wird die Website automatisch aktualisiert.


# Header und Footer erstellen
Header.jsx

> function Header() {
> 
>   return (
> 
>     <header>
  
>       <a href="./home.html">Home </a>
>  
>       <a href="./project.html">Our Project </a>
> 
>       <a href="./mosquitoes.html">Why Mosquitoes suck (literally!) </a>
> 
>       <a href="./NBP.html">How NBP can help </a>
> 
>     </header>
> 
>   );
> 
> }
> 
> export default Header;

Footer.jsx

> function Footer() {
>
>   return (
>
>     <>
>
>       <a href="./contact.html">Contact </a>
>
>       <a href="./language.html">Language </a>
>
>       <>&copy; iGEM Muenster 2024 </>
>
>     </>
>
>   );
>
> }
>
> export default Footer;

App.jsx

> import ComponentName from "./ComponentName.jsx";
> 
> import Header from "./Header.jsx";
> 
> import Footer from "./Footer.jsx";
> 
>
> function App() {
> 
>  return (
> 
>    <>
> 
>      <Header />
>
>      <ComponentName />
>
>      <Footer />
>
>    </>
> 
>  );
> 
> }
> 
> export default App;
> 
>


# JavaScript im HTML Code einbinden

