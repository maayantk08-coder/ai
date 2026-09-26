<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Responsive Card Design</title>

    <style>

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: Arial, sans-serif;
            background: #f1f1f1;
        }

        /* HEADER */
        .header {
            background: #d50063;
            color: white;
            text-align: center;
            padding: 12px 10px;
        }

        .header h1 {
            font-size: 64px;
            font-weight: bold;
        }

        /* CARDS AREA */
        .cards-container {
            width: 100%;
            max-width: 1000px;
            margin: 50px auto 65px;

            display: flex;
            justify-content: space-between;
            gap: 36px;
        }

        /* CARD */
        .card {
            background: #eeeeee;
            width: 32%;

            border: 1px solid #ddd;
            border-radius: 8px;

            overflow: hidden;

            box-shadow: 0 1px 3px rgba(0,0,0,0.08);
        }

        /* IMAGE */
        .card img {
            width: 100%;
            height: 205px;
            object-fit: cover;
            display: block;
        }

        /* CARD CONTENT */
        .card-content {
            padding: 14px;
        }

        .card h2 {
            font-size: 26px;
            margin-bottom: 10px;
            color: #111;
        }

        .card p {
            font-size: 14px;
            line-height: 19px;
            color: #666;
            margin-bottom: 14px;
        }

        /* BUTTON */
        .card button {
            background: #333;
            color: white;

            border: none;
            border-radius: 4px;

            padding: 8px 16px;

            font-size: 14px;
            cursor: pointer;
        }

        .card button:hover {
            background: #555;
        }

        /* FOOTER */
        .footer {
            background: #000;
            color: white;

            text-align: center;
            padding: 15px;
        }

        .footer h2 {
            font-size: 70px;
        }

        /* RESPONSIVE */
        @media (max-width: 800px) {

            .header h1 {
                font-size: 45px;
            }

            .cards-container {
                flex-wrap: wrap;
                padding: 0 20px;
            }

            .card {
                width: 48%;
            }

            .footer h2 {
                font-size: 50px;
            }
        }

        @media (max-width: 600px) {

            .header h1 {
                font-size: 32px;
            }

            .cards-container {
                flex-direction: column;
                align-items: center;
                margin-top: 30px;
            }

            .card {
                width: 100%;
                max-width: 400px;
            }

            .footer h2 {
                font-size: 36px;
            }
        }

    </style>
</head>

<body>

    <!-- HEADER -->
    <header class="header">
        <h1>RESPONSIVE CARD DESIGN</h1>
    </header>


    <!-- CARDS -->
    <main class="cards-container">

        <!-- CARD 1 -->
        <div class="card">

            <img src="https://images.unsplash.com/photo-1454496522488-7a8e488e8606?auto=format&fit=crop&w=800&q=80"
                 alt="Mountain">

            <div class="card-content">

                <h2>Card 1</h2>

                <p>
                    Lorem ipsum dolor sit amet, consectetur
                    adipisicing elit, sed do eiusmod tempor
                    incididunt ut labore et dolore magna aliqua.
                </p>

                <button>Read More</button>

            </div>
        </div>


        <!-- CARD 2 -->
        <div class="card">

            <img src="https://images.unsplash.com/photo-1500534623283-312aade485b7?auto=format&fit=crop&w=800&q=80"
                 alt="Mountain">

            <div class="card-content">

                <h2>Card 2</h2>

                <p>
                    Lorem ipsum dolor sit amet, consectetur
                    adipisicing elit, sed do eiusmod tempor
                    incididunt ut labore et dolore magna aliqua.
                </p>

                <button>Read More</button>

            </div>
        </div>


        <!-- CARD 3 -->
        <div class="card">

            <img src="https://images.unsplash.com/photo-1464822759023-fed622ff2c3b?auto=format&fit=crop&w=800&q=80"
                 alt="Mountain">

            <div class="card-content">

                <h2>Card 3</h2>

                <p>
                    Lorem ipsum dolor sit amet, consectetur
                    adipisicing elit, sed do eiusmod tempor
                    incididunt ut labore et dolore magna aliqua.
                </p>

                <button>Read More</button>

            </div>
        </div>

    </main>


    <!-- FOOTER -->
    <footer class="footer">
        <h2>Using Flexbox</h2>
    </footer>

</body>
</html>
