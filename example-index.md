---
layout: default
title: Your Project Name
description: Your project description here
---

<!-- 
This is a template for your script-generated landing page content.
Your script should:
1. Parse README.md for project information
2. Generate the HTML content below
3. Replace this content with the generated HTML body
4. Keep the frontmatter above unchanged

The Jekyll theme provides:
- Tailwind CSS (already loaded)
- Navigation header with docs integration
- Footer
- Dark/light theme toggle
- Auto-generated documentation navigation

Your script-generated HTML should include the main content sections
like hero, features, installation, etc.
-->

<section class="py-20 sm:py-24 lg:py-32">
    <div class="container mx-auto px-4 sm:px-6 lg:px-8 text-center">
        <h1 class="text-4xl sm:text-5xl lg:text-6xl font-extrabold text-stone-900 dark:text-white tracking-tight">Your Project</h1>
        <div class="mt-6 prose-styles max-w-3xl mx-auto">
            <p>Your project description from README.md goes here.</p>
        </div>
        
        <!-- Your script should generate buttons like this -->
        <div class="mt-10 flex flex-wrap flex-col sm:flex-row justify-center items-center gap-4">
            <a href="#features" class="inline-block rounded-lg bg-sky-600 px-8 py-3 text-base font-semibold text-white shadow-sm hover:bg-sky-700 transition-colors">Get Started</a>
            <a href="/docs/" class="inline-flex items-center justify-center bg-white dark:bg-stone-700 px-6 py-3 text-base font-semibold text-sky-600 dark:text-sky-400 shadow-sm ring-1 ring-inset ring-stone-300 dark:ring-stone-600 hover:bg-stone-100 dark:hover:bg-stone-600 transition-colors rounded-lg">Documentation</a>
            <a href="https://github.com/your-username/your-repo" target="_blank" class="inline-flex items-center justify-center bg-stone-700 hover:bg-stone-800 text-white px-6 py-3 text-base font-semibold shadow-sm rounded-lg transition-colors">GitHub</a>
            <a href="https://gitingest.com/your-username/your-repo" target="_blank" class="inline-flex items-center justify-center bg-sky-700 hover:bg-sky-800 text-white px-6 py-3 text-base font-semibold shadow-sm rounded-lg transition-colors">Ingest</a>
            <a href="https://deepwiki.com/your-username/your-repo" target="_blank" class="inline-flex items-center justify-center bg-green-600 hover:bg-green-700 text-white px-6 py-3 text-base font-semibold shadow-sm rounded-lg transition-colors">Deep Wiki</a>
        </div>
    </div>
</section>

<!-- Your script should generate sections like this from README.md content -->
<section id="features" class="py-16 sm:py-20 lg:py-24 bg-white dark:bg-stone-800">
    <div class="container mx-auto px-4 sm:px-6 lg:px-8">
        <div class="text-center">
            <h2 class="text-3xl font-bold tracking-tight text-stone-900 dark:text-white sm:text-4xl">Features</h2>
        </div>
        <!-- Features content from README.md -->
    </div>
</section>

<section id="installation" class="py-16 sm:py-20 lg:py-24 bg-stone-50 dark:bg-stone-900">
    <div class="container mx-auto px-4 sm:px-6 lg:px-8">
        <div class="text-center">
            <h2 class="text-3xl font-bold tracking-tight text-stone-900 dark:text-white sm:text-4xl">Installation</h2>
        </div>
        <!-- Installation content from README.md -->
    </div>
</section>