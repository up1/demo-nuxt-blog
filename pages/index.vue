<script setup lang="ts">
import type { Blog } from '~/types';

 const blogList: Blog[] = [
    {
      id: 1,
      title: 'Blog 1',
      description: 'Desscription of blog 1',
      tags: ['tag 1', 'tag 2'],
      username: 'Somkiat Pui',
      createdDate: '2024/05/02',
      favoritesCount: 100,
    },
    {
      id: 2,
      title: 'Blog 2',
      description: 'Description of blog 2',
      tags: ['tag 3', 'tag 4'],
      username: 'Somkiat Pui',
      createdDate: '2024/05/01',
      favoritesCount: 200,
    }
  ];
</script>

<template>
  <div>

    <Head>
      <title>Home — Demo</title>
    </Head>
    <AppHome />
    <MyContainer>
      <div class="flex md:space-x-4">
        <!-- List of blogs -->
        <div class="md:w-3/4 mr-4">
          List of blogs
          <BlogList :blogs="blogList" />
        </div>
        <!-- Popular tags -->
        <div class="md:w-1/4 mt-2">
          <div class="sidebar p-3 rounded bg-gray-100">
            <p class="mb-2 text-sm font-medium">Popular Tags</p>
            <ul class="tag-list list-none">
              <li class="mr-1 mb-1 inline-block">
                <Tag name="tag 1" class="tag text-white bg-gray-400" />
              </li>
              <li class="mr-1 mb-1 inline-block">
                <Tag name="tag 2" class="tag text-white bg-gray-400" />
              </li>
              <li class="mr-1 mb-1 inline-block">
                <Tag name="tag 3" class="tag text-white bg-gray-400" />
              </li>
              <li class="mr-1 mb-1 inline-block">
                <Tag name="tag 4" class="tag text-white bg-gray-400" />
              </li>
              <li class="mr-1 mb-1 inline-block">
                <Tag name="tag 5" class="tag text-white bg-gray-400" />
              </li>
            </ul>
          </div>
        </div>
      </div>
    </MyContainer>
  </div>
</template>