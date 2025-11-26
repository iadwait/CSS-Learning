<div class="pricing">
    <div class="card">
        <h2>Basic</h2>
        <p>$9/mo</p>
        <button>Choose</button>
    </div>
    <div class="card featured">
        <h2>Pro</h2>
        <p>$19/mo</p>
        <button>Choose</button>
    </div>
    <div class="card">
        <h2>Enterprise</h2>
        <p>$49/mo</p>
        <button>Choose</button>
    </div>
</div>

<style>
    .pricing {
        display: flex;
        gap: 20px;
        justify-content: center;
        padding: 40px;
        background: rgb(239, 239, 243);
    }
    .card {
        flex: 1 1 250px;
        border: 0.5px solid black;
        border-radius: 10px;
        padding: 20px;
        text-align: center;
        transition:
            transform 0.25s ease,
            box-shadow 0.25s ease;
    }
    .card:hover {
        transform: translateY(-8px);
        box-shadow: 0 8px 20px rgba(0, 0, 0, 0.15);
    }
    .featured {
        background: #e9f3ff;
        border: 2px solid #007aff;
    }
    @media (max-width: 900px) {
        .pricing {
            flex-direction: column;
        }
    }
</style>

