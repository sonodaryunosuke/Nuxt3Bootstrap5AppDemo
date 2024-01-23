<template>
  <div>
    <TrainingPlanList
      :exercises="exercises"
      :selectedExercise="selectedExercise"
      @updateSelectedExercise="updateSelectedExercise"
    />
    <TrainingPlanDetails :exercise="selectedExercise" />
  </div>
</template>

<script>
import TrainingPlanList from './components/TrainingPlanList.vue';
import TrainingPlanDetails from './components/TrainingPlanDetails.vue';

export default {
  data() {
    return {
      exercises: [
        { id: 1, name: "大胸筋" },
        { id: 2, name: "三頭筋" },
        // 他のトレーニングデータ
      ],
      selectedExercise: null,
    };
  },
  methods: {
    updateSelectedExercise(exercise) {
      this.selectedExercise = exercise;
    },
  },
  components: {
    TrainingPlanList,
    TrainingPlanDetails,
  },
};
</script>
