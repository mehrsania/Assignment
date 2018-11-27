<template>
  <table class="table">
    <thead>
      <tr>
        <th>Title</th>
        <th>Subtitle</th>
        <th>Body</th>
        <th>Image</th>
      </tr>
    </thead>
    <tbody>
      <tr v-for="card in cards" class="active">
        <td>{{ card.title }}</td>
        <td>{{ card.subtitle }}</td>
        <td>{{ card.body }}</td>
        <td><img style="width:100%" v-bind:src="card.imgSrc" /></td>
      </tr>
    </tbody>
  </table>
</template>

<script>
export default {
  name: "gbc-table",
  props: [],
  data() {
    return {
      cards: [
        {
          title: "CN Tower",
          subtitle: "Best place ever",
          body: "The food is pretty bad but the view is great",
          imgSrc:
            "https://www.torontobusco.com/wp-content/uploads/2017/05/n-dd-600x400.jpg"
        },
        {
          title: "Niagara Falls CA",
          subtitle: "Second best",
          body: "The food is horrible but the view is decent",
          imgSrc:
            "https://media-cdn.tripadvisor.com/media/photo-s/0f/73/db/0a/niagara-falls-boat-tour.jpg"
        },
        {
          title: "Niagara Falls US",
          subtitle: "Second best",
          body: "The food is horrible but the view is decent",
          imgSrc:
            "https://media-cdn.tripadvisor.com/media/photo-s/0f/73/db/0a/niagara-falls-boat-tour.jpg"
        },
        {
          title: "CN Tower",
          subtitle: "Best place ever",
          body: "The food is pretty bad but the view is great",
          imgSrc:
            "https://www.torontobusco.com/wp-content/uploads/2017/05/n-dd-600x400.jpg"
        },
        {
          title: "Niagara Falls CA",
          subtitle: "Second best",
          body: "The food is horrible but the view is decent",
          imgSrc:
            "https://media-cdn.tripadvisor.com/media/photo-s/0f/73/db/0a/niagara-falls-boat-tour.jpg"
        },
        {
          title: "Niagara Falls US",
          subtitle: "Second best",
          body: "The food is horrible but the view is decent",
          imgSrc:
            "https://media-cdn.tripadvisor.com/media/photo-s/0f/73/db/0a/niagara-falls-boat-tour.jpg"
        }
      ]
    };
  }
};
</script>
