<script setup></script>

<template>
  <main>
    <div
      class="container bg-[url('../../public/favicon.ico')] bg-no-repeat bg-cover"
    >
      <div class="flex flex-col md:flex-row gap-3">
        <div class="customFlex">01</div>
        <div class="customFlex">02</div>
        <div class="customFlex">03</div>
      </div>
      <div class="@2xl bg-slate-500 py-4 rounded-full text-white my-5">
        <article class="not-prose px-5 truncate underline">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Eveniet
          quisquam earum deleniti. Necessitatibus, totam animi saepe veniam
          dolore sequi aliquid!
        </article>
      </div>

      <button
        class="px-4 py-2 font-semibold text-sm bg-blue-500 text-white rounded-md shadow-sm hover:-translate-y-1 hover:scale-110 hover:bg-indigo-500 ease-in-out delay-150 duration-300"
      >
        Save Changes
      </button>
      <p class="truncate w-48">
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Error
        reprehenderit amet ducimus repudiandae, eius aut laborum provident in
        ipsam ab?
      </p>

      <fieldset class="p-4">
        <legend>Published status</legend>

        <input
          id="draft"
          class="peer/draft"
          type="radio"
          name="status"
          checked
        />
        <label for="draft" class="peer-checked/draft:text-sky-500">Draft</label>

        <input
          id="published"
          class="peer/published"
          type="radio"
          name="status"
        />
        <label for="published" class="peer-checked/published:text-sky-500"
          >Published</label
        >

        <div class="hidden peer-checked/draft:block">
          Drafts are only visible to administrators.
        </div>
        <div class="hidden peer-checked/published:block">
          Your post will be publicly visible on your site.
        </div>
      </fieldset>
    </div>
  </main>
</template>
