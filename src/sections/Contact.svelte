<script>
    import emailIcon from "../assets/images/email-icon.svg"
    import linkedinIcon from "../assets/images/linkedin-icon.svg"
</script>

<div id="contact" class="container">
    <div class="contact">
        <h2>Contact</h2>
        <div class="contact-item">
            <img class="icon" src={emailIcon} alt="google icon">
            <span>talfedev@gmail.com</span>
        </div>
        <a class="contact-item" href="#contact">
            <img class="icon" src={linkedinIcon} alt="linkedin icon">
            <span>Linkedin</span>
        </a>
    </div>
</div>

<style>
    .container {
        background-color: #dadada;
        padding: 60px 0;
    }

    .contact {
        margin: 0 auto;
        max-width: 1200px;
        padding: 0 20px;
    }

    .contact-item {
        display: flex;
        align-items: center;
        gap: 10px;
        margin-bottom: 20px;
        font-size: 1.5rem;
    }

    h2 {
        margin-bottom: 50px;
    }

    .icon {
        width: 35px;
        height: 35px;
    }

    a {
        color: black;
    }
</style>