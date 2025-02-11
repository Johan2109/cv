<template>
  <div
    class="min-h-screen bg-gray-50 text-gray-900 dark:bg-gray-900 dark:text-white transition-all duration-300"
  >
    <HeaderSection />
    <main class="container mx-auto p-4 max-w-8xl">
      <ProfileSection />
      <KnowledgeSection />
      <EducationSection />
      <ExperienceSection />
      <ReferencesSection />
    </main>
    <AppFooter />
  </div>
</template>

<script>
import HeaderSection from "./../components/HeaderSection.vue";
import ProfileSection from "./../components/ProfileSection.vue";
import KnowledgeSection from "./../components/KnowledgeSection.vue";
import EducationSection from "./../components/EducationSection.vue";
import ExperienceSection from "./../components/ExperienceSection.vue";
import ReferencesSection from "./../components/ReferencesSection.vue";
import AppFooter from "../components/AppFooter.vue";

export default {
  components: {
    HeaderSection,
    ProfileSection,
    KnowledgeSection,
    EducationSection,
    ExperienceSection,
    ReferencesSection,
    AppFooter,
  },
};
</script>
