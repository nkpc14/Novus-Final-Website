<template>
    <div class="landingPage">
        <Header/>
        <MainSectionGrid/>
        <Approach class="Approach"/>
        <EventSection class="EventSection"/>
        <ProjectSection/>
        <ContactUsSection/>
    </div>
</template>

<script>
    import MainSectionGrid from "./LandingPage/MainSectionGrid";
    import Approach from './Approach/Approach';
    import Header from './LandingPage/Header';
    import EventSection from './Events/EventSection';
    import ProjectSection from './Projects/ProjectsSection';
    import ContactUsSection from './ContactUs/ContactUsSection';
    export default {
        name: "LandingPage",
        components: {
            MainSectionGrid,
            Approach,
            Header,
            EventSection,
            ProjectSection,
            ContactUsSection
        },
    }
</script>

<style scoped lang="scss">
    .landingPage{
        background-color:#262334;
        min-height: 100vh;
        color: #fff;
        font-size: 1.6rem;
        height: auto;
        width: 100%;
        overflow-x: hidden;
    }

    .Approach{
        margin-top: 10rem;
    }

    .EventSection{
        margin-top: 30rem;
    }
</style>
