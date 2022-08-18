<template>
  <div>
    <h1>Заполните форму</h1>
    <form>
      <h3>Информация об университете</h3>

      <Input
          v-model="event.nameOfTheUniversity"
          label="Название университета"
          type="text"
          class="field"
      />
      <Input
          v-model="event.nameOfTheFaculty"
          label="Название факультета"
          type="text"
          class="field"
      />

      <Input
          v-model="event.nameOfTheDepartament"
          label="Специальность"
          type="text"
          class="field"
      />

      <h3>Информация об экзаменаторе</h3>

      <Input
          v-model="event.TheExaminerLastName"
          label="Фамилия"
          type="text"
          class="field"
      />

      <Input
          v-model="event.TheExaminerFirstName"
          label="Имя"
          type="text"
          class="field"
      />

      <Input
          v-model="event.TheExaminerMiddleName"
          label="Отчество"
          type="text"
          class="field"
      />

      <h3>Данные о председателе цикловой комиссии</h3>

      <Input
          v-model="event.TheChairmanLastName"
          label="Фамилия"
          type="text"
          class="field"
      />

      <Input
          v-model="event.TheChairmanFirstName"
          label="Имя"
          type="text"
          class="field"
      />
      <Input
          v-model="event.TheChairmanMiddleName"
          label="Отчество"
          type="text"
          class="field"
      />

      <h3>Специальность и предмет</h3>

      <Input
          v-model="event.SpecialtyСode"
          label="Код специальности"
          type="number"
          class="field"
      />
      <Input
          v-model="event.NameOfTheSpecialty"
          label="Название специальности"
          type="text"
          class="field"
      />

      <Input
          v-model="event.SubjectName"
          label="Название предмета"
          type="text"
          class="field"
      />

      <h3>Вопросы</h3>

      <Input
          v-model="event.theoreticalQuestion"
          label="Теоретические вопросы"
          type="text"
          class="field"
      />
      <Input
          v-model="event.practicalQuestions"
          label="Практические вопросы"
          type="text"
          class="field"
      />
    </form>
  </div>
</template>

<script>
import Input from "@/components/Input";
export default {
  components: {Input},
  data() {
    return {
      event: {
          nameOfTheUniversity: '',
          nameOfTheFaculty: '',
          nameOfTheDepartament:'',

        TheExaminerLastName: '',
        TheExaminerFirstName: '',
        TheExaminerMiddleName: '',

        TheChairmanLastName: '',
        TheChairmanFirstName: '',
        TheChairmanMiddleName: '',

        SpecialtyСode: '',
        NameOfTheSpecialty: '',

        SubjectName: '',

        practicalQuestions: [],
        theoreticalQuestion: []

      }
      }
      }
    }
</script>

<style scoped>
</style>