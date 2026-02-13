body {
    margin: 0;
    padding: 0;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
    background: linear-gradient(135deg, #0f2027 0%, #203a43 50%, #2c5364 100%);
    font-family: 'Nunito', sans-serif;
    overflow: hidden;
}

/* Screen 1: The Proposal */
#proposal-screen {
    text-align: center;
    z-index: 10;
    padding: 20px;
}

h1 {
    color: #4da6ff;
    font-family: 'Dancing Script', cursive;
    font-size: 3.5rem;
    margin-bottom: 30px;
    text-shadow: 2px 2px 8px rgba(0,0,0,0.3);
}

.btn-container {
    position: relative;
    height: 100px;
    display: flex;
    justify-content: center;
    gap: 20px;
}

button {
    font-size: 1.2rem;
    padding: 12px 30px;
    border: none;
    border-radius: 50px;
    cursor: pointer;
    font-weight: bold;
    transition: transform 0.2s ease, background 0.3s ease;
    box-shadow: 0 4px 15px rgba(0,0,0,0.3);
}

/* YES Button */
#yesBtn {
    background-color: #1e90ff;
    color: white;
}

#yesBtn:hover {
    transform: scale(1.1);
    background-color: #4da6ff;
}

/* NO Button */
#noBtn {
    background-color: white;
    color: #1e90ff;
    position: absolute;
}

/* Screen 2: The Letter */
#letter-screen {
    display: none;
    position: relative;
    width: 100%;
    height: 100vh;
    justify-content: center;
    align-items: center;
    padding: 20px;
    box-sizing: border-box;
    overflow-y: auto;
}

.paper {
    background-color: #ffffff;
    width: 100%;
    max-width: 500px;
    padding: 40px;
    border-radius: 15px;
    box-shadow: 0 15px 40px rgba(0,0,0,0.3);
    position: relative;
    animation: fadeInUp 1s ease forwards;
    text-align: left;
    line-height: 1.6;
    color: #333;
    margin: auto;
    border-left: 6px solid #1e90ff;
}

.paper h2 {
    font-family: 'Dancing Script', cursive;
    color: #1e90ff;
    font-size: 2.5rem;
    margin-top: 0;
    text-align: center;
}

.signature {
    font-family: 'Dancing Script', cursive;
    font-size: 1.8rem;
    margin-top: 30px;
    text-align: right;
    color: #1e90ff;
}

/* Animations */
@keyframes fadeInUp {
    from { opacity: 0; transform: translateY(20px); }
    to { opacity: 1; transform: translateY(0); }
}

/* Confetti */
.confetti {
    position: absolute;
    width: 10px;
    height: 10px;
    background-color: #1e90ff;
    animation: fall linear forwards;
}

@keyframes fall {
    to { transform: translateY(100vh) rotate(720deg); }
}
<div class="paper">
    <h2>To My Mandipa 💙</h2>

    <p>
        From the very beginning, you have been my calm in the chaos and 
        my strength when I needed it most. I don’t think you even realize 
        how much your presence alone makes everything feel lighter.
    </p>

    <p>
        You have this quiet confidence, this way of protecting, loving, 
        and caring that makes me feel safe in a way I never knew I needed. 
        With you, I don’t have to pretend. I don’t have to be anything 
        other than myself.
    </p>

    <p>
        I love the way you think. I love the way you speak. 
        I love the way you carry yourself like a man who knows who he is. 
        And most of all, I love how you love me.
    </p>

    <p>
        No matter where life takes us, I want you to always remember 
        that you are deeply appreciated, deeply respected, and deeply loved.
    </p>

    <p>
        Thank you for being my peace, my best friend, 
        and my favorite person.
    </p>

    <div class="signature">
        Forever yours,<br>
        Courtney 💙
    </div>
</div>
