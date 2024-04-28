<script>
    let location = {
        floorId : "00"
    }


</script>

<h1 class="text-gradient">Location Component (svelte)</h1>

Stockwerk auswählen:

<select bind:value={location.floorId}  name="location" id="location">
    <option value={"00"}>Default</option>
    <option value={"01"}>Obergeschoss 1</option>
    <option value={"02"}>Obergeschoss 2</option>
    <option value={"03"}>Obergeschoss 3</option>
    <option value={"04"}>Obergeschoss 4</option>
    <option value={"05"}>Obergeschoss 5</option>
    <option value={"U1"}>Untergeschoss 1</option>
    <option value={"U2"}>Untergeschoss 2</option>
</select>
<p >
    Location_No: 8600-Dübendorf-Zürichstrasse 30-<span class="yellow">{location.floorId}</span>-B440
</p>
<style>


    select {
        margin-left: 20px;
        font-size: 1rem;
        padding: 10px;
        min-width: 200px;
        border-radius: 5px;
    }

  .yellow{
    color: yellow;
  }
</style>