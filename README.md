**SIW**

De Bartolo Diego: 177116 & Sparano Francesco: 184530

Progetto Web Computing
----------------------

Descrizione:

Foodify è un applicazione web che permette la creazione, visualizzazione e
gestione di un ristorante. L’utente può accedere al sito dei diversi ristoranti
presenti sulla piattaforma, sfogliare il menu scegliere i prodotti desiderati ed
effettuare un ordine.

**Analisi dei requisiti:**

**Utente**

1.  deve poter visuale l’offerta gastronomica corrente

2.  autenticarsi sulla piattaforma

3.  aggiungere e gestire i prodotti nel proprio carrello

4.  visualizzare lo storico dei suoi ordini

5.  effettuare un ordine e decidere il metodo di consegna, ritiro o domicilio,
    pagamento alla consegna o con carta

**Gestore**

1.  il sistema deve notificare al gestore l’ordine effettuato

2.  deve poter registrare un ristorante sulla piattaforma

3.  modificare i dettagli e la grafica del sito

4.  modificare, gestire visualizzare gli ordini del suo ristorante

**Casi d’uso:**

1.  Visualizzazione del catalogo di ogni ristorante registrato,
    Indipendentemente dalla sessione il sito dovrà offrire all’utente, oltre ad
    informazioni riguardo al locale, la possibilità di consultare le offerte
    gastronomiche del ristorante, queste offerte saranno di vario genere (pizze,
    contorni, speciali) dinamiche e aggiornate dal gestore tramite la pagina di
    amministrazione del locale

2.  Effettuare un’ordinazione L’utente dovrà essere in grado di effettuare il
    login tramite le sue credenziali oppure tramite Google, selezionare elementi
    dal catalogo da aggiungere al proprio carrello, visualizzare gli elementi
    nel carrello, modificare la quantità di ogni articolo selezionato,
    effettuare l’ordine scegliendo la consegna a domicilio o il ritiro così come
    il metodo di pagamento.

3.  Creazione di un Locale sulla piattaforma con la possibilità di specificare
    tutti i dettagli relativi all’attività cosi come modificare la grafica del
    proprio sito,

4.  Gestione del locale creato, nello specifico degli ordini ricevuti, il
    gestore ha la possibilità di modificare lo stato di avanzamento degli ordini
    tramite un apposita pagina di gestione, dei prodotti offerti dal locale, il
    gestore avrà la possibilità di aggiungere ingredienti e prodotti alla
    propria offerta gastronomica

**Librerie ed API utilizzate:**

-   Lato client l’applicazione utilizza HTML5, CSS, e Javascript/JQuery

-   Vengono utilizzati oggetti JSON per ricevere informazioni dal database

-   L’applicazione utilizza Ajax per la comunicazione di dati e updates tra
    client e server.

-   Viene utilizzata l’API Google Sign-In per l’autenticazione degli utenti

-   Viene utilizzata l’API Stripe per effettuare i pagamenti tramite carta di
    credito

-   Il sistema utilizza Bootstrap per la gestione grafica e delle Animazioni ed
    è possibile utilizzare l’applicazione su sistemi mobile in quanto si
    dimostra full responsive.

**Package, Classi e pagine create**

Pagine:

-   about.html

-   ChooseLocal.html

-   ConfermaUtente.hml

-   Contact.html

-   index.html

-   Login.html

-   menu_1.html

-   MyAccount.html

-   Sign-In.html

Classi:

**Package classes:** (Package che contiene le servlet )

-   Address.java

-   addtoCart.java

-   AllProducts/AllAnalytic/AllIngredients/AllLocals/AllLogs/AllOrders/AllTypeOfProduct/AllUsers/AllUsersByConfirm.java
    *(classi utilizzate principalmente per la visualizzazione e la gestione
    dello stato del ristorante)*

-   DecreaseQuantityProduct.java / IncreaseQuantityProduct.java

-   ConfermaUtente.Java

-   CreateLocal.Java

-   DeleteOrder.java

-   GetCart.java

-   IngredientById.java

-   IngredientsOfProduct.java

-   isLogged.java

-   isRestaurantchosen.java (se non è stato ancora selezionato un ristorante
    porta alla pagina di selezione)

-   LocalBySession.java

-   LocalInfo

-   Login.java

-   Logout.java

-   OrdersById / OrdersByProduct / OrdersByState / OrdersByUser.java

-   ProductsByOrder/ProductsByType.java

-   SaveAnalitic / SaveLog / SaveNewsletter / SaveOrder / SaveProduct /
    SaveReview / SaveUser.java

-   SendMail.java

-   tokenSignin.java

-   UpdateLocal / UpdateLoggedUser / UpdateOrder / UpdateProduct.java

-   UserById.java

**Package dao**: (Package che gestisce il login e la sessione)

-   IngredientDAO.java

-   AnalyticDAO.java

-   LogDAO.java

-   NewsletterDAO.java

-   OrderDAO.java

-   ProductDAO.java

-   RestaurantDAO.java

-   ReviewProductDAO.java

**Package DataBase**: (Package che comprende le classi interne principali del
sistema)

-   DBConnection.java

-   AnalyticDaoJDBC.java

-   idBroker.java

-   IngredientDaoJDBC.java

-   LogDaoJDBC.java

-   NewsLetterDaoJDBC.java

-   OrderDaoJDBC.java

-   PersistenceException.java

-   ProductDaoJDBC.java

-   RestaurantDaoJDBC.java

-   ReviewLocalDaoJDBC.java

-   ReviewProductDaoJDBC.java

-   TypeDaoJDBC.java

-   UserDaoJDBC.java

**Package model**: (package di logica interna all’applicazione)

-   Analytic.java

-   Cart.java

-   Email.java

-   Ingredient.java

-   Log.java

-   Order.java

-   Product.java Restaurant.java

-   Review.java

-   ReviewLocal.java

-   ReviewProduct.java

-   State.java

-   Type.java

-   User.java
