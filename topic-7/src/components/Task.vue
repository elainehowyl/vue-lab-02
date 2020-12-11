<template>
  <div class="card" style="width: 18rem">
    <div class="card-body">
      <h5 class="card-title">{{ task.name }}</h5>
      <ul>
        <li>Date Due: {{ task.dateDue }}</li>
        <li>Urgency: {{ task.urgency }}</li>
        <li>Importance: {{ task.importance }}</li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
    props:['task']
}
</script>
