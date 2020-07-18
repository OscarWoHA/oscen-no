<template>
    <div>
        <section id="top">
            <header>
                <img src="/profile.jpg" />
                <h1>
                    <strong>hello,</strong>
                    <br />my name's Oscar
                </h1>
                <p>
                    <a href="mailto:ohalland@gmail.com">and I'm a developer and entrepeneur</a>
                </p>
            </header>
        </section>
    </div>
</template>

<script>
</script>

<style lang="scss" scoped>
    #top {
        display: flex;
        flex-direction: row;

        justify-content: center;
        align-items: center;

        min-height: 100vh;
        min-height: --webkit-fill-available;
    }

    #scroll {
        position: fixed;

        bottom: 0;

        font-weight: 300;

        color: rgba(0, 0, 0, 0.5);
    }

    header {
        display: flex;
        flex-direction: column;

        color: #1d3557;

        position: relative;

        > img {
            height: 100%;
            width: auto;

            overflow: hidden;

            position: absolute;

            left: -35%;   
            bottom: -75%; 

            z-index: -1;    
        }

        > h1 {
            font-weight: 400;
            font-size: 3rem;

            line-height: 1.1;

            margin: 0 0 0.5rem 0;

            > strong {
                font-weight: 300;
                font-size: 2rem;
            }
        }

        > p {
            font-weight: 300;
            font-size: 1.25rem;

            align-self: flex-end;

            margin: 0;

            padding-bottom: 0.5rem;

            border-bottom: 2px solid #e63946;

            > a {
                text-decoration: none;
                color: inherit;
            }
        }
    }
</style>
