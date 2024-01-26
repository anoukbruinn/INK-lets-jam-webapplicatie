<script>

</script>

<main>
<div class="mainScreen">
    <!-- <img src="https://image.freepik.com/free-vector/purple-background-with-neon-frame_52683-34124.jpg" class="bgimg" alt=""> -->
    <div class="card">
        <div class="leftSide">
            <img
                src="/assets/ink.png"
                class="product"
                alt="Shoes"
            />
        </div>
        <div class="rightSide">
            <form action="">
                <h1>CheckOut</h1>
                <h2>Payment Information</h2>
                <p>Cardholder Name</p>
                <input type="text" class="inputBox" name="name" required />
                <p>Donation Option</p>
                <select class="inputBox" name="card_type" id="card_type" required>
                    <option value="">--Select a option--</option>
                    <option value="Visa">Material</option>
                    <option value="RuPay">Financial</option>
                    <option value="MasterCard">Clothing</option>
                </select>

                <p>Card Number</p>
                <input type="number" class="inputBox" name="card_number" id="card_number" required />

                <p>Card Type</p>
                <select class="inputBox" name="card_type" id="card_type" required>
                    <option value="">--Select a Card Type--</option>
                    <option value="Visa">Visa</option>
                    <option value="RuPay">Discovery</option>
                    <option value="MasterCard">MasterCard</option>
                </select>
                <div class="expcvv">
                    <p class="expcvv_Text">Expiry</p>
                    <input type="date" class="inputBox" name="exp_date" id="exp_date" required />
                    <p class="expcvv_Text2">CVV</p>
                    <input type="cc-csc" class="inputBox" name="cvv" id="cvv" required />
                </div>
                <p>Amount</p>
                <div style="display: flex;">
                    <span style="margin-right: 5px;">$</span>
                    <input type="number" class="inputBox" name="amount" id="amount" required />
                </div>
                <p></p>
                <form action="/Paymentgood" method="get">
                    <button type="submit" class="button">
                     CheckOut
                    </button>
                  </form>
                  
            </form>
        </div>
    </div>
</main>

<style>

/* Main Screen Layout */
.mainScreen {
    min-height: 100vh;
    width: 100%;
    display: flex;
    flex-direction: column;
    margin-top: 10%;
    background-color: var(--Charcoal);
    color: var(--Charcoal);
    font-family: var(--Apercu-Font)
}

/* Card Styling */
.card {
    width: 60rem;
    margin: auto;
    background: white;
    border-radius: 1.5rem;
    box-shadow: 4px 3px 20px #3535358c;
    display: flex;
    flex-direction: row;
}

/* Left Side Styling */
.leftSide {
    width: 25rem;
    display: flex;
    align-items: center;
    justify-content: center;
    border-top-left-radius: 1.5rem;
    border-bottom-left-radius: 1.5rem;
}

/* Product Image */
.product {
    object-fit: cover;
    width: 20em;
    height: 20em;
    border-radius: 100%;
}

/* Right Side Styling */
.rightSide {
    background-color: var(White);
    width: 35rem;
    border-bottom-right-radius: 1.5rem;
    border-top-right-radius: 1.5rem;
    padding: 1rem 2rem 3rem 3rem;
}

/* Paragraph Styling */
p {
    display: block;
    font-size: 1.1rem;
    font-weight: 400;
    margin: .8rem 0;
}

/* Input Box Styling */
.inputBox {
    color: #030303;
    width: 100%;
    padding: 0.5rem;
    border: none;
    border-bottom: 1.5px solid #ccc;
    margin-bottom: 1rem;
    border-radius: 0.3rem;
    font-family: var(--Apercu-Font);
    color: #615a5a;
    font-size: 1.1rem;
    font-weight: 500;
    outline: none;
}

/* CVV Section Styling */
.expcvv {
    display: flex;
    justify-content: space-between;
    padding-top: 0.6rem;
}

.expcvv_Text {
    padding-right: 1rem;
}

.expcvv_Text2 {
    padding: 0 1rem;
}

/* Button Styling */
.button {
    background: var(--Yellow-Primary);
    color: var(--Charcoal);
    padding: 15px;
    border: none;
    border-radius: 50px;
    font-weight: 400;
    font-family: var(--Apercu-Font);
    font-size: 1.2rem;
    margin-top: 10px;
    width: 100%;
    letter-spacing: .11rem;
    outline: none;
}

/* Button Hover Effect */
.button:hover {
    transform: scale(1.05) translateY(-3px);
    box-shadow: 3px 3px 6px #38373785;
}

/* Responsive Design */
@media only screen and (max-width: 1000px) {
    .card {
        flex-direction: column;
        width: auto;
    }

    .leftSide {
        width: 100%;
        border-top-right-radius: 0;
        border-bottom-left-radius: 0;
        border-top-right-radius: 0;
        border-radius: 0;
    }

    .rightSide {
        width: auto;
        border-bottom-left-radius: 1.5rem;
        padding: 0.5rem 3rem 3rem 2rem;
        border-radius: 0;
    }
}


/* Styling for Valid Input */
.inputBox:valid {
    border-bottom-color: green; /* Change border color on valid input */
}

</style>