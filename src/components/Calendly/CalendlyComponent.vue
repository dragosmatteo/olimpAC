<script setup>
import SportCard from "./components/SportCard.vue";
import Fotbal from "./../../assets/img/football.png";
import Biliard from "./../../assets/img/biliard.jpg";
import PingPong from "./../../assets/img/pingpong.jpg";
import Badminton from "./../../assets/img/badminton.jpg";
import Volei from "./../../assets/img/volei.jpg";
import Chess from "./../../assets/img/chess.jpg";
import Table from './../../assets/img/table.jpg'
import Remi from './../../assets/img/remi.jpg'
</script>

<template>
  <div class="max-w-[1140px] m-auto" id="calendar">
    <h1
      class="text-white text-center text-[32px] sm:text-[32px] md:text-[56px] lg:text-[56px] xl:text-[56px] font-syne font-bold leading-none w-full"
    >
      Calendar Eveniment <br />
      <span class="text-yellow">2024</span>
    </h1>

    <div
      class="grid grid-cols-1 sm:grid-cols-1 md:grid-cols-2 gap-x-[24px] gap-y-[40px] pt-[120px]"
    >
      <SportCard
        title="Fotbal"
        text="Run for your team and make it easy. Fotbalul este un joc de echipă - odată ce echipa și-a stabilit pozițiile și energia, mingea poate fi urmărită și ghidată spre un gol ce poate face diferența în ultimul minut."
        :imageSrc="Fotbal"
        locatie="TBA"
        data="25 Mai (Finala 26 Mai)"
      />
      <SportCard
        title="Biliard"
        text="Biliardul, un joc îndrăgit de studenți este un moment în care jucătorii își arată îndemânarea și finețea. În așteptarea rândului propriu, printre bile și tac se strecoară și discuții care vor lega prietenii, deși doar unul dintre cei doi jucători va merge mai departe."
        :imageSrc="Biliard"
        locatie="TBA"
        data="23 Mai"
      />
      <SportCard
        title="Ping Pong"
        text="Mingile sunt aruncate, iar jucătorii răspund provocării adversarului. Ce trebuie să facă este să lase mingea în cădere o singură dată în terenul propriu și să o trimită imediat celuilalt. Câștigă cel care prezintă concentrare, reflexe agere și adună punctajul maxim: enjoy the ping-pong sound."
        :imageSrc="PingPong"
        locatie="TBA"
        data="24 Mai"
      />
      <SportCard
        title="Badminton"
        text="Un fluturaș, două rachete și dorința de distracție sunt rețeta unui joc de succes în interior sau în aer liber, dar și o idee perfectă pentru doza de mișcare. Obiectivul jocului este de a ține fluturașul în limitele terenului și a-l face să cadă pe terenul oponentului."
        :imageSrc="Badminton"
        locatie="TBA"
        data="26 Mai"
      />
      <SportCard
        title="Volei"
        text="Un salt pentru minge înseamnă un salt pentru echipă. Voleiul este mai mult decât un joc, este o legătură între coechipieri și un moment trăit împreună ce îi unește spre același scop: victoria echipei."
        :imageSrc="Volei"
        locatie="TBA"
        data="26 Mai"
      />
      <SportCard
        title="Sah"
        text="&quot;Chess is everything: art, science and sport.&quot;
         Pentru a câștiga este nevoie de câțiva pași pe tabla de șah, însă atunci când vezi o mișcare bună, caută una și mai bună, indiferent de ce piesă alegi să folosești împotriva adversarului tău.
        It&apos;s not over until you win."
        :imageSrc="Chess"
        locatie="TBA"
        data="26 Mai"
      />
      <SportCard
        title="Table"
        text="Old, but gold: jocul de table, învățat de mulți în copilărie, rămâne unul dintre cele mai dorite activități. Zarurile sunt aruncate, piesele se adună în casă și se scot afară. Competiția este strânsă: primul care reușește este declarat câștigător, be quick!"
        :imageSrc="Table"
        locatie="TBA"
        data="26 Mai"
      />
      <SportCard
        title="Remi"
        text="Cu oponenți aleși sau nu, totul depinde de participant și de ce piese are pe tablă. Regulile sunt simple: scapă de duble și caută să cobori piesele pe tablă în suite sau perechi. Punctele adunate ne anunță câștigătorul, trust the process"
        :imageSrc="Remi"
        locatie="TBA"
        data="26 Mai"
      />
    </div>
  </div>
</template>

<style>
.main-title {
  color: #2d2d2d;
  text-align: center;
  text-transform: capitalize;
  padding: 0.7em 0;
}
</style>
