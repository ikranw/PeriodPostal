<script>
  let organizations = [
    {
      name: "The Pachamama Project",
      img: "/public/pproject.png",
      shipsTo: "Refugee camps and communities in Uganda, Ukraine, Pakistan, Italy, South Sudan, Lebanon, Greece, and more",
    },
    {
      name: "The Pad Project",
      img: "/public/TPP_Logo.png",
      shipsTo: "Internationally to countries like Kenya, Uganda, Sierra Leone, Ghana, India, Guatemala, and more",
    }
  ];

  let forumPosts = [
    {
      userName: "Amina",
      userImg: "/public/user2.jpg",
      date: "Wednesday, December 10th, 2025",
      country: "United States",
      message: "I need menstrual products of 2–4 pads and the shipping location address is 1234 postal office.",
    },
    {
      userName: "Sara",
      userImg: "/public/user1.jpg",
      date: "Friday, December 5th, 2025",
      country: "Lebanon",
      message: "I need sewing materials and cotton fabric. The shipping location address is 2323 postal office.",
    },
    {
      userName: "Ikran",
      userImg: "/public/user3.jpg",
      date: "Friday, December 5th, 2025",
      country: "Somalia",
      message: "I need sweing materials and 4–8 resuable pads. The shipping location address is 2525 postal office.",
    }
  ];
</script>

<div class="mail-page">

  <section class="org-section">
    <h2 class="section-title">Organizations to Mail to: </h2>

    <div class="org-list">
      {#each organizations as org}
        <div class="org-card">
          <img src={org.img} alt={org.name} class="org-img" />
          <div class="org-info">
            <h3 class="org-name">{org.name}</h3>
            <p class="org-ship-label">Ships to:</p>
            <p class="org-ship-location">{org.shipsTo}</p>
          </div>
        </div>
      {/each}
    </div>
  </section>

  <section class="forum-section">
    <h2 class="section-title">Community Forum:</h2>

    <div class="forum-list">
      {#each forumPosts as post}
        <div class="forum-card">
          <div class="forum-header">
            <img src={post.userImg} alt={post.userName} class="user-img" />
            <div class="user-info">
              <p class="user-name">{post.userName}</p>
              <p class="post-date">{post.date} | {post.country}</p>
            </div>
          </div>
          <div class="post-message">
            <p>{post.message}</p>
          </div>
        </div>
      {/each}
    </div>
  </section>

</div>

<style>
  @import "../app.css";

  .mail-page {
    max-width: 900px;
    margin: 0 auto;
    padding: 2rem 1.5rem 3rem;
    display: flex;
    flex-direction: column;
    gap: 2.5rem;
  }

  .section-title {
    font-size: 1.6rem;
    font-weight: 700;
    color: #ff4f9a;
    margin-bottom: 1.2rem;
    text-align: left;
  }

  .org-list {
    display: flex;
    flex-direction: column;
    gap: 1.2rem;
  }

  .org-card {
    display: flex;
    gap: 1rem;
    align-items: center;
    background-color: #ffe3f0;
    border-radius: 10px;
    padding: 1rem;
    box-shadow: 0 4px 10px rgba(255, 79, 154, 0.15);
  }

  .org-img {
    width: 70px;
    height: 70px;
    object-fit: cover;
    border-radius: 8px;
  }

  .org-info {
    display: flex;
    flex-direction: column;
    gap: 0.25rem;
  }

  .org-name {
    font-size: 1.1rem;
    font-weight: 700;
    margin: 0;
    color: #000000;
  }

  .org-ship-label {
    font-size: 0.9rem;
    font-weight: 600;
    margin: 0;
    color: #000000;
  }

  .org-ship-location {
    font-size: 0.95rem;
    margin: 0;
    color: #272626;
  }

  .forum-section {
    margin-top: 1rem;
  }

  .forum-list {
    display: flex;
    flex-direction: column;
    gap: 1rem;
  }

  .forum-card {
    background-color: #ffffff;
    border-radius: 10px;
    padding: 1rem;
    box-shadow: 0 4px 10px rgba(155, 9, 9, 0.05);
    display: flex;
    flex-direction: column;
    gap: 0.75rem;
    border: 1.5px solid #ffdde6;
  }

  .forum-header {
    display: flex;
    gap: 0.75rem;
    align-items: center;
  }

  .user-img {
    width: 50px;
    height: 50px;
    border-radius: 50%;
    object-fit: cover;
  }

  .user-info {
    display: flex;
    flex-direction: column;
  }

  .user-name {
    font-weight: 700;
    margin: 0;
    color: #000000;
  }

  .post-date {
    font-size: 0.85rem;
    color: #666666;
    margin: 0;
  }

  .post-message p {
    margin: 0;
    font-size: 0.95rem;
    line-height: 1.5;
    color: #000000;
  }
</style>
