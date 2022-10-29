<template>
    <div class="c-contact" id="contact">
       <div class="text-contact">
        © RAK SUSHI 2022&nbsp;&nbsp;•&nbsp;&nbsp;25110 Prachin Buri&nbsp;,&nbsp;Kabin Buri,&nbsp;Nong Ki&nbsp;67/266&nbsp;&nbsp;•&nbsp;&nbsp;Tel: 095-1342883&nbsp;&nbsp;•&nbsp;&nbsp;Delicious,&nbsp;clean,&nbsp;hygienic. <br><br>
        •&nbsp;&nbsp;FB:Apirak Namrak&nbsp;&nbsp;•&nbsp;&nbsp;E-mail: 6306021420132@fitm.kmutnb.ac.th&nbsp;&nbsp;<br>•&nbsp;&nbsp;Tel: 095-1342883
       </div>
    </div>
</template>

<script>
export default {
  name: 'C-Contact'
}
</script>

<style>

.c-contact{
    width: 100%;
    height: 20vh;
    background: rgb(37, 37, 37);
    color: #fff;
    font-family: var(--font-text);
    position: relative;
    bottom: 0;
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;
}

@media (max-width: 740px) {
  
.text-contact{
  font-size: 10px;
  
}
}
</style>