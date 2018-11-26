<template>
  <div>
    <table class="table">
      <my-tablehead
        titlehead="Title"
        subtitlehead="Subtitle"
        bodyhead="Body"
        imghead="Picture"
      >
      </my-tablehead>

      <tbody v-for="card in cards" class="table">
        <my-row v-bind="card"></my-row>
      </tbody>
    </table>

    <div>
      <div style="padding-bottom: 150px">
        <div class="container">
          <div class="columns">
            <div v-for="card in cards" class="column col-4">
              <my-card v-bind="card"></my-card>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import MyCard from "./components/card.vue";
import MyRow from "./components/row.vue";
import MyTablehead from "./components/tablehead.vue";

export default {
  name: "App",
  components: {
    MyCard,
    MyRow,
    MyTablehead
  },
  data() {
    return {
      cards: [
        {
          title: "CN Tower",
          subtitle: "Beautiful view",
          body: "Food is bad, but the view is pretty",
          imgSrc:
            "https://www.torontobusco.com/wp-content/uploads/2017/05/n-dd.jpg"
        },
        {
          title: "Eiffel tower",
          subtitle: "Looks awesome",
          body: "View is breathtaking",
          imgSrc:
            "https://www.smartertravel.com/uploads/2016/03/France-ParisEiffelTowerfromBelow-DD.jpg"
        },
        {
          title: "Burj Khalifa",
          subtitle: "Tallest in the world!",
          body: "I'll visit one day",
          imgSrc:
            "https://assets.isango.com/productimages/product/12042/dubai_25801_1.jpg"
        }
      ]
    };
  }
};
</script>
