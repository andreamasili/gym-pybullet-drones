# Una difesa smorta dello status quo.   
  
## Intro  
  
  
Arriva un momento nella vita di ognuno in cui diventa d'obbligo scrivere un articolo di difesa dello status quo.  
Questo mio intervento mi battezza come conservatore tecnologico dopo anni di tecno-ottimismo.   
  
Meglio, quindi, mostrare issare subito i colori delle mie bandiere per identificare meglio da quale pulpito sta arrivando la predica:   
Sono nato nel segno della bilancia con ascendente right-libertarian, sono vagamente competente in ambito tech e ignoro sostanzialmente l'intero mondo finanziario per il quale provo innato disgusto e paura.    
  
Voglio un sistema resistente alla censura, non mi piace l'idea di delegare a terzi la possibilità di formare un giudizio su un evento/testo/etc.  
Voglio un sistema neutrale di pagamenti! Le sconce signorine di OnlyFans non meritano l'esclusione dai circuiti bancari o simili. (PayPal, Etc.)    
Voglio un sistema innovativo: Il COBOL nelle banche è una piaga sociale da debellare.   
Voglio un sistema sicuro: Il COBOL nelle banche è una piaga sociale da debellare.  
Voglio un sistema decentralizzato che possa permettere tutte queste cose.   
Possibilmente non manipolabile.   
  
Dovrei essere un evangelista per Web3/Crypto/DAO/NFTs  
  
Ma non lo sono. Questo è il riassunto del mio viaggio nell'ecosistema cripto!  
   
   
## Do I need a blockchain?  
#### La soluzione in cerca di un problema.  
  
Non ho mai capito la fascinazione col definire la blockchain come un'invenzione particolarmente moderna: I Merkle Trees sono stati brevettati nel 1979, le Hash Chain sono abbastanza vecchie da averle viste insieme alle linked list ancora 10/15 anni fa.   
Ma essere strutture dati vecchie non significa essere inutili (anche le reti neurali sono state teorizzate nel 1943, backpropagation nel 1975, etc...)  
Quindi, vediamo se questa struttura dati contemporanea di Shining si rivela essere veramente l'ingrediente fondamentale per curare i problemi della società moderna.   
  
D'altronde, i poteri dichiarati dallo sfruttamento di questa innovativa tecnologia sono parecchi ( https://www.sofi.com/learn/content/benefits-of-crypto/  ).   
  
La quantità di video, post che si possono trovare per declamare i pregi di questa invenzione sono difficili da sottostimare.   
Questo è già un testo abbastanza lungo e dovrò fare anch'io quello che fanno in moltissimi nell'ambiente crypto: dar per scontato che siano noti i termini e, in caso di errore mio, fingere superiorità e dire "non intendo quello, è una semplificazione!"  
  
Vediamo il funzionamento di una blockchain:   
  
In essenza e in una semplificazione un pò barbara, una blockchain è una struttura dati append-only in cui ogni blocco contiene l'informazione legata all'hash del blocco precedente.  
Questo permette, "validando" un blocco, di validare anche tutti i precedenti!   
L'esempio più blando di una blockchain: un server GIT con SHA-256 firma l'head ad ogni pull request: la nostra blockchain privata! 
  
La blockchain delle criptovalute non è privata, invece, è trustless e pubblica:  
Non c'è alcuna autorità, l'unica autorità sui dati inseriti nella blockchain viene dal consenso dei nodi.   
Questo aggiunge delle complicazioni ma, fondamentalmente, la struttura rimane: un registro o ledger append-only in cui le aggiunte possono essere validate tramite un consenso della rete che partecipa.  
  
Se il ledger contiene lo storico di transazioni tra utenti del tipo   
Alice paga a Bob 50 TRABICCOLI, firmato Alice.   
Bob paga a Caio 25 TRABICCOLI, firmato Bob.   
  
ecco che nasce una criptovaluta. (suppongo che il lettore di questo pezzo abbia già idea di come funzioni veramente)  
  
Dunque: ammettendo di avere un sistema di consenso efficiente, il resto è un sistema efficiente?  
  
Non particolarmente e non per design: in un mondo in cui nessuno si fida di nessun'altro, ognuno deve possedere la copia del ledger per poter risalire al saldo di ognuno per poter verificare da sè la correttezza dell'hash.   
Questo porta ad una moltiplicazione enorme e livelli enormi di rindondanza di dati. Per design.   
Ad oggi, la blockchain di Bitcoin è più o meno sui 320 gigabytes ( https://fortunly.com/statistics/blockchain-statistics/ )*  
Questo è un problema arcinoto di Bitcoin: non è scalabile.   
  
Cosa si è fatto per risolvere il problema?   
Bitcoin ha limitato la crescita ad 1MB a blocco. Questo non senza problemi sulla velocità del sistema: il sistema riesce a gestire dalle 3 alle 7 transazioni al secondo globalmente... Mica male.   
  
Ma quando si parla di sprechi legati a bitcoin, difficilmente quello di memoria è quello che sale nei titoli di giornali.   

  
## Proof of Nothing.   
#### Proof of Work? Proof of Waste is more like it.   
  
Per il vero spreco, purtroppo, bisogna guardare ai sistemi di consenso della rete.   
Per premiare i nodi che validano le transazioni, ad ogni transazione viene "generato" o "minato" dei bitcoin.   
Il sistema di consenso più utilizzato è il celebre Proof of Work.  
Il pc che valida la soluzione deve risolvere per primo una serie di operazioni per trovare l'hash giusto.   
Questo consegue in un una competizione winner-takes-all in cui chi spende di più in corrente/capacità di calcolo/GPU/ASIC/etc riesce a vincere il "premio".   
Questo è degenerato in un sistema gonfio che consuma più o meno tanta corrente quanto la Thailandia intera.  (per gestire dalle 3 alle 7 transazioni al secondo...)  
  
  
Fortunatamente la soluzione è stata pensata: 
> proof of Stake risolverà tutto!
     
Ethereum, nel suo whitepaper, annuncia il passaggio a questa innovativa forma per risolvere i numerevoli problemi di bitcoin!   
  
si decide con una lotteria pesata sul numero di token/coin chi scriverà il nuovo blocco sulla blockchain e le fees verranno a loro assegnate!   
Se non altro, non sarà più necessario consumare la corrente della Thailandia: rapido progresso!   
  
Questo schema ha problemi facilmente prevedibili anche da me? Yep!  
Se uno ha molti token statisticamente prenderà più blocchi (e quindi più fees) aumentando la loro chance di essere ripescati e aumentando il loro controllo della rete.  
Una volta raggiunto il 51%, diventano sovrani della chain.   
Qualche simpatico miliardario/fondo d'investimento può assumere rapidamente il controllo della rete mentre avrebbe fatto più fatica a trovare la valanga di GPU o ASIC necessari ad acquisire il controllo della rete PoW.  
  
>Ma Delegated Proof of Stake risolverà tutto:
   
Ma con Proof of Stake attaccare la rete sarà svantaggioso per l'attaccante! Non ha senso spendere per prendere il 51% dei token per poi devastare il sistema!  
Facile argomentare che non serve devastare l'ecosistema per agire in maniera losca e comunque mantenere la gente dentro al circuito: blocco le transazioni del mio rivale Gino ma non di tutto il resto o simili esempi.   
  
>Ma lo slashing sarà da garanzia:  

Con slashing si intende penalizzare il nodo che produce blocchi invalidi. Questo, chiaramente, funziona solo se l'attaccante è un idiota ed è sotto al 51%.  
     
>Ma con Proof of BOH succederà X e Y:
   
Il problema è trovare un consenso tra nodi non fidati etc: è un problema abbastanza complesso che ha i suoi trade-off e probabilmente ci sarà una soluzione prima o poi... forse?   
  
La mia è una difesa smorta dello status quo attuale, quindi mi pare solo che giusto confrontarlo col sistema web3 attualmente in circolazione e dominante.
E non con una potenziale forma migliorata nel futuro (che sta sempre dietro l'angolo) 

## Is this worth it?  
  
Quindi, tornando a noi, l'attuale sistema, per quanto lento, dispendioso ed inefficiente è una buona garanzia contro la decentralizzazione?  

I principali mining pool di Bitcoin (con più del 50% del controllo della rete) sono 5.   
Ethereum ha 3 mining pool con più del 50% di controllo della rete.   
  
Il dibattito su questo punto non sfugge, ovviamente, all'ambiente crypto: https://www.coindesk.com/markets/2014/06/20/are-51-attacks-a-real-threat-to-bitcoin/  
  
I fork in BTC non sono eventi incredibili, Ethereum stesso ha dovuto eseguirne uno per "salvare" da il risultato infelice di uno smart contract, separandosi in Ethereum e Ethereum classic.   
  
Ma vabbè, se la blockchain non è innovativa, non è una garanzia di decentralizzazione, può salvarsi con gli sviluppi di DeFi, dApp e analoghi?
   
  
## Ethereum e Web3  
#### Il macchinario infernale  
Ignorare i problemi delle fondamenta per andare a verificare i piani superiori non è un saggio consiglio ingegneristico, però magari ci sono degli sviluppi interessanti!    
Ethereum, in particolare, ha fatto nascere un'ecosistema di sviluppi basati sulla celebre Ethereum Virtual Machine.  
Il sistema dona la possibilità di "far girare" codice su un sistema distribuito.  
Questi programmi anche il nome di smart contract.    
  
Questo dona la possibilità, anche, la nuova frontiera del web! Web3!     

In web3 non ci saranno autorità centrali, non ci sarà censura, avremo un metodo verificabile per poter conservare documenti, cartelle cliniche, patenti etc!   
Basta gatekeeper alla google, basta con la tirannia di AWS di Amazon!  
D'altronde, il perchè web3 merita di essere considerato anch'esso ha innumerevoli evangelisti ( https://future.a16z.com/why-web3-matters/ )  
  
Vediamo, dunque, una applicazione di web3: la nostra nuova dApp  
  
Intanto, guardiamo la base della nostra dApp: La Ethereum Virtual Machine.  
Ogni operazione di questa EVM ha un costo in GAS   
il costo per OPCODE è riportato in questo documento  
https://docs.google.com/spreadsheets/d/1n6mRqkBz3iWcOlRem_mO09GtSKEKrAsfO7Frgx18pNU/edit#gid=0  
    
Una addizione tra interi viene 3 unità di GAS.    
    
https://ethstats.net/ ci può dare molte informazioni interessanti.     
    
Al momento della scrittura: c'è un blocco ogni 12 secondi e 1 unità di gas costa 77.11 Gwei che equivalgono circa a 0.0002 $ USD    
Ogni blocco può avere una quantità di gas limitato dal voto della rete.     
Quindi, ad esempio, con i numeri attuali, 12500000/3/12 = 350000 IPS di addizioni.    
  
  
ETH EVM è una macchina a 0,350 MIPS (million instructions per seconds)    
Per confronto, un raspberry PI 2 è sui 4,500 MIPS.     
Son circa 200 dollari al secondo che vengono lanciati in gas per eseguire le istruzioni.     
  
La nostra dApp parte su un sistema abbastanza scadente, però potrà solo che migliorare, quindi vediamo l'architettura che questo ecosistema consiglia:   
  
https://www.preethikasireddy.com/post/the-architecture-of-a-web-3-0-application    
  
Vediamo se questo è un passo avanti rispetto allo status quo.     
  
Ricordiamo, che, in tutto questo, il design è della blockchain di peer: un client normale con il suo browser non è fattibile come nodo (un full node richiede 600GB, e comunque contiene solo gli ultimi N blocchi della blockchain, quindi non può verificare effettivamente l'intero ledger)    
L'unico modo per interagire con la blockchain è che questa stia su dei server da qualche altra parte.    
E questi server che si sono i peer della rete.
Tra di loro c'è l'ambiente trustless, pubblico, anonimo.  


Noi, mortali, per interagire con la blockchain dobbiamo fare uso di servizi esterni.   
Fortunatamente per noi, sono nate delle aziende che permettono di accedere ai nodi di questa rete: e.g. Infura/Alchemy.    
  
Queste aziende ci offrono API, servizi di dati, analytics e tante altre cose. (ah, dejavù)   
Per interagire con la blockchain, quindi, la nostra dApp manda una richiesta ad Infura, Infura risponde con un amalgama di JSON con scritto "Ecco cosa dice il risultato dell'operazione su blockchain" e la dApp mostra il risultato.     
(ah, fun fact, i risultati della chiamata all'API di Infura non sono nemmeno signed. +1 Trusted Gatekeeper)     

> Ma esistono alternative ad Infura! Pokt invece firma le risposte!
 
Ha la stessa energia di "DuckDuckGo non blocca i risultati": vero, ma non è il big player. 
  

Chiaramente sviluppare una rete globale su una macchina 20 volte più scarsa di un singolo Raspberry potrebbe non scalare.   
Fortunatamente per la nostra dApp, nascono altri servizi per permettere al sistema di scalare. (e giù di altri gatekeeper) 
  
  
Dal documento sopra, notiamo che salvare in memoria un intero a 256bit viene a costare 20.000 unità di GAS (circa 6/7 euro, a prezzi attuali)  
Fortunatamente, ci sono altri servizi di storage da poter aggiungere più o meno decentralizzati per ovviare al problema! (+1 Gatekeeper)    






Per poi gestire l'equivalente del login, nasce un'altro gatekeeper sottoforma di Metamask.  
https://github.com/MetaMask !
  
Metamask, tra l'altro, per funzionare deve interagire con la blockchain!     
Per visualizzare le transazioni, ad esempio,  Metamask chiama l'API di Etherscan    
e per visualizzare il totale del wallet? yep, chiamata all'API di Infura.    
E per visualizzare gli NFT? yep, chiamata all'API di OpenSeas!    
  
Rainbow wallet, magari?     
https://github.com/rainbow-me/rainbow/tree/b7078dfa398059717e1a1b9c417e80d95b2c73c8#readme    
Anche loro chiamano Infura, Etherscan e altri sempre soliti noti.     
  
  
Questi non sono altro che ulteriori gatekeeper e layer aggiuntivi per aggirare il punto centrale che la EVM NON è ora una alternativa decente.  
Ma magari ha il potenziale! 
  
## Presto per giudicare  
#### Ma abbastanza tardi per difendere senza entusiasmo il sistema attuale 
"Ma è un sistema nella sua infanzia! è presto per giudicare!"      
Il whitepaper di Ethereum è del 2014.     
il whitepaper di Bitcoin è del 2008.    
  
In un certo senso sì, nonostante siano passati circa 10 anni posso accettare il fatto che sia relativamente nuovo come ambiente.  
Questo, però, non è di grande consolazione: fin dall'infanzia, potrei dire, il sistema ha dimostrato una rapidissima tendenza alla centralizzazione e la maggiorparte dell'ecosistema francamente se ne frega.  

  
I problemi dell'attuale sistema sono particolarmente noti al fondatore di Ethereum:   
> For a blockchain to be decentralized, it's crucially important for regular users to be able to run a node, and to have a culture where running nodes is a common activity. https://vitalik.ca/general/2021/05/23/scaling.html   
  
Quindi, magari, nel 2023 con Sharding e Proof of Stake, l'ecosistema ethereum diventerà davvero il beacon di speranza necessario e non uno scomodo sistema arcano utilizzato per permettere blanda speculazione finanziaria.  
Ma, fino a quel momento, propongo la mia smorta difesa allo status quo.  
  
Per hostare un server nell'attuale sistema bisogna contrattare con un host.  
Si trovano host che hostano anche i nazisti.
Gli host sono entità individuabili di cui uno può sfruttare il libero mercato per "fidarsi".
Gli host sono vari e non sono ancora fortemente centralizzati (anche se la direzione è quella).  
C'è vaga pluralità: se voglio hostare winnie the pooh, hosto in USA  
Se voglio hostare le nefandezze del figlio di Biden, un host in cina o in russia è ben contento di offrirmi servizi di host.  
Le uniche cose difficili da hostare sono materiale pedopornografico o cose illegali in ogni parte del mondo: una limitazione ragionevole.  


   
## Il problema non è tecnico.   
#### Il problema di web2 non è tecnico, è di natura umana. 
Web2 è verso la centralizzazione da un sistema decentralizzato di web1: la gente non vuole gestire server, pochissimi nerd hanno la volontà di scriversi il proprio server di posta.
La centralizzazione di servizi è avvenuta in maniera naturale anche con protocolli decentralizzati (il protocollo delle mail è decentralizzato, ad esempio, anche se gmail diventa monopolista)
Aggiungere ulteriori layer e complicazioni non cambierà il problema di fondo: far girare un server http è oltre il del 99% degli utenti del web. 

OpenSeas potrebbe fornire un servizio nettamente migliore abbandonando tutto il carrozzone web3: fees più convenienti e anche un log pubblico con più trasparenza.   
Chiaramente, però, agli investitori di NFT, questo non è di minimo interesse: il valore sta nella parola magica Crypto. 
Non nella resistenza alla censura (visto che i celebri NFT spariscono nel vuoto)  
Non nella sicurezza.   
Non nella decentralizzazione.    
  
## Un rapido sguardo all'ecosistema
#### E la natura umana fa schifo
Data l'ingestibilità tecnica sia di Bitcoin che di Ethereum (fees assurde, tempi di transazione eterni) sono nati, appunto, tonnellate di progetti crypto alternativi.   
Sia sopra alla rete di smart contract descritti sopra e sia come valute crypto alternative per permettere di essere schermati o dalla volatilità o dalla lentezza/ingestibilità.  
Di questi progetti crypto, uno non può fare a meno di notare l'evidente speedrun di tutte le truffe finanziarie ed economiche conosciute nella storia dell'uomo:   
dalla crisi dei tulipani (NFT), alle banche del farwest (Tether) ai più improbabili schemi di Ponzi, l'ecosistema è un postribolo di truffe rimarchevoli.  
  
Naturalmente, ogni DAO regolata da smart contract diventa un serie di bug bounty potenzialmente da milioni e, visto che Code is Law, il codice scritto con le limitazioni sopra riportate è l'equivalente di lanciare un contratto scritto da singole persone in una vasca di avvocati squali.   
(Che poi è quello che è successo con la primissima DAO, the DAO)  
  
Da semi-sviluppatore, posso garantire che il codice marcisce, il codice si rompe e "Code is Law" è uno scenario della società non troppo desiderabile.   
  
Ma è un buon motivo per essere scettici dell'ecosistema? da un punto di vista tecnico sarebbe un non sequitur   
  
Da un punto di vista sociale: magari sì, per come la vedo: la direzione di un ecosistema non viene solo dall'idealismo dichiarato da persone come Vitalik o Balaji Srinivasan, viene anche dalla spinta economica degli investitori.
E per la maggioranza degli investitori il core tecnico è una sfida da aggirare per proporre la nuova truffa, il nuovo servizio. 

In futuro potrebbe cambiare ma il futuro deve arrivare, quindi per il momento, godiamoci la disgrazia altrui con il grift counter di https://web3isgoinggreat.com/ e debelliamo il COBOL dalle banche.



  
  
