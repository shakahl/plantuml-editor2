<script setup lang="ts">
import { useAddUmlCode } from '@/usecase/UseAddUmlCode'

const { addNewUmlCOde } = useAddUmlCode()
</script>

<template>
  <li class="nav-item dropdown">
    <span class="nav-link dropdown-toggle" role="button" data-bs-toggle="dropdown">Template</span>
    <ul class="dropdown-menu position-absolute">
      <li><span class="dropdown-header">behavioral diagrams</span></li>
      <li><span class="dropdown-item" role="button" @click="addNewUmlCOde('usecaseTemplate')">Use Case</span></li>
      <li><span class="dropdown-item" role="button" @click="addNewUmlCOde('activitybTemplate')">Activity &#946;</span></li>
      <li><span class="dropdown-item" role="button" @click="addNewUmlCOde('activityTemplate')">Activity</span></li>
      <li><span class="dropdown-item" role="button" @click="addNewUmlCOde('sequenceTemplate')">Sequence</span></li>
      <li><hr class="dropdown-divider" /></li>
      <li><span class="dropdown-header">structural diagrams</span></li>
      <li><span class="dropdown-item" role="button" @click="addNewUmlCOde('objectTemplate')">Object</span></li>
      <li><span class="dropdown-item" role="button" @click="addNewUmlCOde('classTemplate')">Class</span></li>
      <li><span class="dropdown-item" role="button" @click="addNewUmlCOde('erTemplate')">ER diagram</span></li>
    </ul>
  </li>
</template>

<style scoped></style>
