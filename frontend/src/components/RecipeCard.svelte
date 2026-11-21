<script lang="ts">
  const recipe = 
    {
      id: 1,
      name: "Creamy Tuscan Chicken",
      image: "https://images.unsplash.com/photo-1532550907401-a500c9a57435?w=600",
      tags: [{ name: "Dinner" }, { name: "Chicken" }]
    };
  const tags = recipe.tags;
</script>

<li class="recipe-card">
  <a href="/recipe/{recipe.id}/">
    <img src={recipe.image} alt={recipe.name} />

    <h2 class="recipe_name">{recipe.name}</h2>

    <div class="recipe-tags">
      {#each tags as tag}
        <span class="recipe-tag">{tag.name}</span>
      {/each}
    </div>
  </a>
</li>

<style>
    /* Recipe Cards */

.recipe-list {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
  gap: 1.5rem;
  padding: 1rem;
  list-style: none;
}

.recipe-card {
  background-color: var(--light-grey);
  border-radius: 14px;
  overflow: hidden;
  border: 1px solid rgba(93, 58, 0, 0.12);
  box-shadow: 0 3px 10px rgba(93, 58, 0, 0.08);
  transition: transform 0.2s ease, box-shadow 0.2s ease;
}

.recipe-card:hover {
  transform: translateY(-5px);
  box-shadow: 0 8px 18px rgba(93, 58, 0, 0.15);
}

.recipe-card a {
  display: block;
  color: var(--dark-grey);
  text-decoration: none;
}

.recipe-card a:hover {
  color: var(--dark-grey);
  text-decoration: none;
}

.recipe-card img {
  width: 100%;
  height: 200px;
  object-fit: cover;
  display: block;
}

.recipe_name {
  font-family: var(--font-headline);
  font-size: 1.35rem;
  color: var(--primary-color);
  padding: 1rem 1rem 0.25rem;
  margin: 0;
}

.recipe-tags {
  display: flex;
  flex-wrap: wrap;
  gap: 0.5rem;
  padding: 0.75rem 1rem 1rem;
}

.recipe-tag {
  background-color: rgba(155, 136, 22, 0.15);
  color: var(--tertiary-color);
  font-size: 0.75rem;
  font-weight: 600;
  padding: 0.35rem 0.7rem;
  border-radius: 20px;
  text-transform: capitalize;
}
</style>