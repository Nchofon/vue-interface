<templete>
  <div class="col-12 col-md-10 col-lg-7">
    <div class="list-group list-group-flush">
    <div class="list-group-item d-flex align-items-start" v-for="(item, i) in appointments" v-bind:key="i" >
      <h4>{{item.petName}}</h4>
      <p>{{item.aptNotes}}</p>
    </div>
    </div>
  </div>
</templete>
<script>
  export default {
    name: "AppointmentList",
    props: ["appointments"]
  };
</script>