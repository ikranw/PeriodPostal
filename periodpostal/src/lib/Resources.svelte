<script>
  let originVid = "Origin video";
  let instructVid = "Instructional video";

  let orginLink = "https://www.youtube.com/watch?v=4ygEJafeHC0";
  let instructLink = "https://www.youtube.com/watch?v=311dZyYttD8";
</script>

<div class="resources-page">
  <h1 class="title">How to make your own handmade pad </h1>

  <div class="videos-section">
    <div class="video-card">
      <div class="video-title">{originVid}</div>
      <div class="video-frame-wrapper">
        <iframe
          src={orginLink}
          title={originVid}
          frameborder="0"
          allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
          allowfullscreen
        ></iframe>
      </div>
    </div>

    <div class="video-card">
      <div class="video-title">{instructVid}</div>
      <div class="video-frame-wrapper">
        <iframe
          src={instructLink}
          title={instructVid}
          frameborder="0"
          allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
          allowfullscreen
        ></iframe>
      </div>
    </div>
  </div>

  <div class="guide-section">
  <h2>
    Reusable Sanitary Pads 
    (credit to:
      <a href="https://www.actionaid.org.uk/sites/default/files/d.i.y._reusable_sanitary_pads.pdf" target="_blank">
        ActionAid
      </a>
    )
  </h2>
   
  <h3 class="pink-title">Materials</h3>
  <ul class="materials-list">
    <li>Thick paper (for template)</li>
    <li>Marker pen</li>
    <li>Ruler</li>
    <li>Scissors</li>
    <li>Thin fabric (cotton is ideal)</li>
    <li>Thick fabric (e.g., an old towel)</li>
    <li>Button</li>
    <li>Needle & thread</li>
    <li>Safety pin</li>
  </ul>

  <h3 class="pink-title">Instructions</h3>
  <ol class="instructions-list">
    <li>Print out the pad template and cut along the dotted line.</li>
    <li>Reverse the material and trace the template over it using a marker. Repeat.</li>
    <li>Using sharp scissors, cut out the two cotton pieces.</li>
    <li>Place one piece on top of the other, with the patterned sides facing each other.</li>
    <li>Sew the sides of the two pieces of fabric together, leaving the top and bottom bits open.</li>
    <li>Turn down the edges of the top and bottom bits and stitch along them, creating a hem.</li>
    <li>Turn the fabric inside out, revealing the pattern and concealing the seams on the inside. Sew up the sides/wings.</li>
    <li>Sew a button in the centre of the right wing.</li>
    <li>Mark on the left wing where you will need a button hole. Cut the hole and sew around the edges to prevent fraying.</li>
    <li>Use a ruler to cut two 20cm long x 6cm wide rectangles from a towel. Lay the pieces on top of each other and sew them together along the top and bottom.</li>
    <li>Attach a large safety pin to the top of the lining. Insert the lining into the casing, using the safety pin to pull it up to the top. Remove the pin.</li>
  </ol>

  <h3 class="pink-title"> Printable Template for Pad & Instructions</h3>
  <p>Download or print the official cutout template here:</p>

  <a 
    href="https://www.actionaid.org.uk/sites/default/files/d.i.y._reusable_sanitary_pads.pdf" 
    class="template-text" 
  >
    https://www.actionaid.org.uk/sites/default/files/d.i.y._reusable_sanitary_pads.pdf
  </a>
</div>
</div>

<style>
 .resources-page {
  max-width: 900px;
  margin: 0 auto;
  padding: 2rem 1.5rem 3rem;
}

.title {
  text-align: center;
  color: #ff4f9a;
  margin-bottom: 2rem;
  font-size: 2.2rem;
}

.videos-section {
  display: flex;
  flex-wrap: wrap;
  gap: 2rem;
  justify-content: center;
  margin-bottom: 2.5rem;
}

.video-card {
  flex: 1 1 320px;
  max-width: 400px;
  background-color: #ffe3f0;
  border-radius: 10px;
  padding: 1rem;
  box-shadow: 0 4px 10px rgba(255, 79, 154, 0.2);
}

.video-title {
  text-align: center;
  font-weight: 600;
  margin-bottom: 0.75rem;
  color: #000000;
}

.video-frame-wrapper {
  position: relative;
  width: 100%;
  padding-bottom: 56.25%;
  border-radius: 8px;
  overflow: hidden;
}

.video-frame-wrapper iframe {
  position: absolute;
  inset: 0;
  width: 100%;
  height: 100%;
}

.guide-section {
  background-color: #ffe3f0;
  padding: 1.8rem;
  border-radius: 10px;
  box-shadow: 0 4px 10px rgba(255, 79, 154, 0.2);
  margin-top: 2rem;
}

.guide-section h2 {
  color: #000000;
  margin-bottom: 1.2rem;
}

.pink-title {
  color: #ff4f9a;
  margin-top: 1.6rem;
  margin-bottom: 0.6rem;
}

.materials-list,
.instructions-list {
  padding-left: 1.5rem;
  line-height: 1.6;
  color: #000000;
  font-weight: 500;
}

.materials-list {
  margin-bottom: 2rem;
}

.guide-section p {
  color: #000000;
  margin-top: 0.4rem;
  margin-bottom: 0.6rem;
}

.guide-section a {
  color: #ffffff;
  text-decoration: underline;
}

.template-text {
  color: #ff4f9a;
  font-weight: 600;
  display: inline-block;
  margin-top: 0.4rem;
}

</style>
