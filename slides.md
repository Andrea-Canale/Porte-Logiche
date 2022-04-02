---
# try also 'default' to start simple
theme: seriph
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: https://source.unsplash.com/collection/94734566/1920x1080
# apply any windi css classes to the current slide
class: 'text-center'
# https://sli.dev/custom/highlighters.html
highlighter: shiki
# show line numbers in code blocks
lineNumbers: false
# some information about the slides, markdown enabled
info: |
  ## Slidev Starter Template
  Presentation slides for developers.

  Learn more at [Sli.dev](https://sli.dev)
# persist drawings in exports and build
drawings:
  persist: false
---

# Porte logiche

Andrea Canale 3^INF


---

# Cosa sono?

<p>Le porte logiche sono dei circuiti integrati che permettono di eseguire delle operazioni booleane</p>
<div align=center>
<img src="/images/not.jpg"/>
</div>
<style>
</style>


---

# Le operaazioni booleane

Le porte logiche appunto ci permettono di svolgere le operazioni booleane che sono:
 <div style="margin-left:500px">
  <ul>
    <li>
L'or è l'operatore booleano "oppure", se negl'ingressi c'è almeno un valore a 1 l'uscita sarà 1
    </li>
    <li>
      L'and logico è l'operatore logico "entrambi", infatti solo se entrambe l'entrate sono a 1 l'uscita sarà 1
    </li>
        <li>
      Il not logico rappresenta la negazione, se in entrata ho 1, in uscita avrò 0 e così via
    </li>
            <li>
      Il NOR è un OR negato, quindi funziona come un OR però inverte i risultati
    </li>
            <li>
      La porta NAND è un AND negato, quindi funziona come un AND ma i risultati sono invertiti
    </li>
                <li>
      La porta XOR o Exclusive-OR dà come risultato 1 solo se uno dei 2 ingressi è 1, se entrambi sono 1 restituirà 0
    </li>
                <li>
      La porta NXOR è uno XOR negato, funziona come uno XOR ma con i risultato invertiti
    </li>
  </ul>
  </div>

 <img src="/images/schema.gif" style="margin-top:-400px" />

 <style>
   li{
     font-size:15px;
     }
   </style>


---


# La porta NOT

<p>La porta NOT come abbiamo detto inverte l'entrata</p>
<p>Ecco qui uno schema con la porta NOT</p>
<div align="center">
<img src="/images/schema.png" width="512"/>
</div>
<p>Come si può vedere nel nostro integrato ogni entrata ha una solo uscita e corrisponde proprio alla porta NOT identificata dal simbolo tra l'ingresso A e l'uscita Y</p>

---


# La porta NOT


<p>La prova del funzionamento con circuito chiuso e aperto</p>

<div grid="~ cols-2 gap-2"  align="center">

<div>
<p>Circuito aperto</p>
<img src="/images/oracceso.png">
</div>
<div>
<p>Circuito chiuso</p>
<img src="/images/orspento.png">
</div>

</div>
<div align="center">
<p>Nel caso del circuito aperto arrivano 0v all'ingresso che la porta invertirà in 5v mentre nel caso del circuito aperto arriveranno 5v nell'ingresso e la porta restituirà 0v in uscita</p>
</div>

---

# La porta AND

<p>La porta AND restituisce 1 solo quando entrambe l'entrate sono 1</p>
<p>Ecco un circuito con una porta AND</p>
<div align="center">
<img src="/images/schemaand.png" width="512"/>
</div>
<p>Anche qui l'integrato ha diverse porte che nello schema vengono identificate con il simbolo AND con 2 entrate ed 1 uscita</p>
---


# La porta AND

<p>La prova del funzionamento con circuito chiuso e aperto</p>

<div grid="~ cols-2 gap-2"  align="center">

<div>
<p>Circuito chiuso</p>
<img src="/images/andaccesa.png">
</div>
<div>
<p>Circuito aperto su uno o più ingressi</p>
<img src="/images/andspenda.png">
</div>

</div>
<div align="center">
<p>Quando in entrambe le entrate passa corrente l'uscità restituirà 5 V mentre se manca la corrente anche in un solo ingresso la portà restituirà 0 V</p>
</div>

---


# La porta OR

<p>La porta OR restituisce 1 quando in almeno una delle entrate passa corrente</p>
<p>Ecco un circuito con una porta OR</p>
<div align="center">
<img src="/images/orvschema.png" width="512"/>
</div>
<p>Anche qui l'integrato ha diverse porte che nello schema vengono identificate con il simbolo OR con 2 entrate ed 1 uscita</p>

---

# La porta OR

<p>La prova del funzionamento con circuito chiuso e aperto</p>

<div grid="~ cols-2 gap-2"  align="center">

<div>
<p>Circuito chiuso su almeno un ingresso</p>
<img src="/images/orvaccesa.png">
</div>
<div>
<p>Circuito aperto su entrambi ingressi</p>
<img src="/images/orvspenta.png">
</div>

</div>
<div align="center">
<p>Quando in almeno una delle entrate passa corrente l'uscità restituirà 5 V mentre se manca la corrente in entrambe la portà restituirà 0 V</p>
</div>


---

# La porta NAND

<p>La porta NAND è un AND negato, ciò significa che restituisce 1 quando entrambe l'entrate sono a 0 e restituisce 0 quando entrambe le entrate sono a 1</p>
<p>Ecco un circuito con una porta NAND</p>
<div align="center">
<img src="/images/schemanand.png" width="512"/>
</div>
<p>Anche qui l'integrato ha diverse porte che nello schema vengono identificate con il simbolo NAND con 2 entrate ed 1 uscita</p>

---

# La porta NAND

<p>La prova del funzionamento con circuito chiuso e aperto</p>

<div grid="~ cols-2 gap-2"  align="center">

<div>
<p>Circuito chiuso su entrambi gli ingressi</p>
<img src="/images/nandchiusa.png">
</div>
<div>
<p>Circuito aperto su uno o più ingressi</p>
<img src="/images/nandaperta.png">
</div>

</div>
<div align="center">
<p>Come si può notare è l'esatto opposto di una AND perchè negata</p>
</div>

---
# La porta AND

<p>La porta NAND è un AND negato, ciò significa che restituisce 1 quando entrambe l'entrate sono a 0 e restituisce 0 quando entrambe le entrate sono a 1</p>
<p>Ecco un circuito con una porta NAND</p>
<div align="center">
<img src="/images/schemanand.png" width="512"/>
</div>
<p>Anche qui l'integrato ha diverse porte che nello schema vengono identificate con il simbolo NAND con 2 entrate ed 1 uscita</p>

---

# La porta NOR

<p>La porta NOR, come la NAND, è una OR negata. Restituisce 1 solo quando entrambi gli ingressi sono a 0 e dà 0 in uscità quando almeno un ingresso è a 1</p>
<p>Ecco un circuito con una porta NOR</p>
<div align="center">
<img src="/images/norschema.png" width="512"/>
</div>
<p>Anche qui l'integrato ha diverse porte che nello schema vengono identificate con il simbolo NOR con 2 entrate ed 1 uscita</p>

---

# La porta NOR

<p>La prova del funzionamento con circuito chiuso e aperto</p>

<div grid="~ cols-2 gap-2"  align="center">

<div>
<p>Circuito chiuso su almeno un ingresso</p>
<img src="/images/norchiuso.png">
</div>
<div>
<p>Circuito aperto su entrambi gli ingressi</p>
<img src="/images/noraperto.png">
</div>

</div>
<div align="center">
<p>Come si può notare è l'esatto opposto di una porta OR perchè negata</p>
</div>

---

# La porta XOR

<p>La porta XOR o exclusive-or è una porta che restituisce 1 se solo una entrata è 1, se entrambe le entrate sono a 1 restuisce 0</p>
<p>Ecco un circuito con una porta XOR</p>
<div align="center">
<img src="/images/xorschema.png" width="512"/>
</div>
<p>Anche qui l'integrato ha diverse porte che nello schema vengono identificate con il simbolo XOR con 2 entrate ed 1 uscita</p>

---

# La porta XOR

<p>La prova del funzionamento con circuito chiuso e aperto</p>

<div grid="~ cols-2 gap-2"  align="center">

<div>
<p>Circuito chiuso su entrambi gli ingressi</p>
<img src="/images/xorchiuso.png">
</div>
<div>
<p>Circuito aperto su 1 ingresso</p>
<img src="/images/xoraperta.png">
</div>

</div>
<div align="center">
<p>La XOR funziona come una OR ma restituisce 1 solo quando c'è solo un ingresso a 1, se entrambi gli ingressi sono a 0 restituisce 0</p>
</div>

---

# La porta NXOR

<p>La porta NXOR è una porta che restituisce 1 se 1 entrambe le entrate hanno lo stesso valore e restuisce 0 solo se una entrata è ad uno</p>
<p>Ecco un circuito con una porta NXOR creata combinando XOR e NOT</p>
<div align="center">
<img src="/images/xorschema.png" width="512"/>
</div>
<!-- <p>Anche qui l'integrato ha diverse porte che nello schema vengono identificate con il simbolo XOR con 2 entrate ed 1 uscita</p> -->

---

# La porta NXOR

