<template>
    <div class="projects">
        <div class="project" v-for="item in projects" :key="item.node.id">
          <a href="https://apps.apple.com/us/app/emoreact/id1477856072?itsct=apps_box&amp;itscg=30200">
            <g-image
                :src="item.node.thumbnail"
                :alt="item.node.title"
                class="thumbnail"
            />
            <h3 class="project-title"></h3>
            <a href="https://apps.apple.com/us/app/emoreact/id1477856072?itsct=apps_box&amp;itscg=30200" style="display: inline-block; overflow: hidden; border-radius: 13px; width: 250px; height: 83px;"><img src="https://tools.applemediaservices.com/api/badges/download-on-the-app-store/black/en-US?size=250x83&amp;releaseDate=1566950400&h=aa895340a99eb0cdf02e7dd24ab5670c" alt="Download on the App Store" style="border-radius: 13px; width: 250px; height: 83px;"></a>
            </a>
        </div>
    </div>
</template>

<script>
export default {
    props: {
        projects: {
            type: Array,
            required: true
        }
    }
}
</script>

<style scoped>
.projects {
  display: grid;
  grid-template-columns: 1fr 1fr;
  grid-gap: 4rem;
}
.project {
  grid-column: auto / span 2;
  text-align: center;
}
.project-link {
  text-decoration: none;
}
.thumbnail {
  height: 560px;
  object-fit: cover;
  transition: all 0.15s ease;
  box-shadow: 0 0 40px -20px rgba(0,0,0,0.25);
}
.project-title {
  font-size: 1rem;
  color: var(--color-contrast);
  margin: 2rem 0 1rem 0;
}
.categories {
  font-size: 0.8rem;
  color: var(--color-contrast-1);
}
.category {
  margin-right: 0.8rem;
}
.category:last-of-type {
  margin: 0;
}
.project:hover .thumbnail {
  transform: scale(1.02);
  box-shadow: 0 20px 40px -20px rgba(0,0,0,0.25);
}

@media (min-width: 920px) {
  .project {
    grid-column: auto / span 1;
  }
  .project:nth-child(3n+1) {
    grid-column: auto / span 2;
  }
}

</style>
