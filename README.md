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
Das kann umgangen werden, indem mehrere HTML Elemente in einem leeren HTML Element (<> </>) eingebettet sind.


Die neu erstellte Komponente muss noch in App.jsx eingebunden werden:

> import ComponentName from "./ComponentName.jsx";
>
> function App() {
>
>   return <ComponentName />;
>
> }
>
> export default App;

Beim Speichern der Datei wird die Website automatisch aktualisiert.

