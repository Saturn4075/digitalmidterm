<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Programmatic Ads & SEO — Interactive MCQ Quiz (Full)</title>
  <style>
    :root{--accent:#4f46e5;--muted:#64748b}
    body{font-family:Inter,ui-sans-serif,system-ui,Arial,Helvetica,sans-serif;background:#f6f8fb;color:#071124;margin:0;padding:28px}
    .card{max-width:1100px;margin:0 auto;background:#fff;border-radius:12px;padding:22px;box-shadow:0 10px 40px rgba(10,20,40,0.06)}
    h1{margin:0 0 6px;font-size:20px}
    p.lead{margin:0 0 18px;color:var(--muted)}
    .topbar{display:flex;justify-content:space-between;align-items:center;gap:12px}
    .progress{height:14px;background:#eef2ff;border-radius:999px;overflow:hidden;flex:1;margin-left:12px}
    .progress > i{display:block;height:100%;background:linear-gradient(90deg,var(--accent),#7c3aed);width:0%}
    .controls{display:flex;gap:10px;align-items:center;margin-top:12px}
    button{background:var(--accent);color:#fff;border:0;padding:8px 12px;border-radius:10px;cursor:pointer}
    button.secondary{background:#eef2ff;color:#071124}
    .grid{display:grid;grid-template-columns:1fr;gap:10px;margin-top:14px}
    .question{padding:12px;border-radius:10px;background:#fbfdff;border:1px solid #eef2ff}
    .qhead{font-weight:600;margin-bottom:8px}
    .opts{display:flex;flex-direction:column;gap:8px}
    label.opt{display:flex;align-items:center;gap:10px;padding:8px;border-radius:8px;background:#fff;border:1px solid #e6eefc;cursor:pointer}
    input[type=radio]{transform:scale(1.05)}
    .feedback{display:none;margin-top:8px;padding:10px;border-radius:8px}
    .feedback.show{display:block}
    .feedback.correct{background:#ecfdf5;color:#065f46;border:1px solid #bbf7d0}
    .feedback.incorrect{background:#fff1f2;color:#9f1239;border:1px solid #fecdd3}
    #result{margin-top:14px;padding:12px;border-radius:10px;background:#f8fafc;border:1px solid #eef2ff}
    footer{margin-top:18px;color:var(--muted);font-size:13px;text-align:right}
    .meta{font-size:13px;color:var(--muted);margin-top:6px}
  </style>
</head>
<body>
  <div class="card">
    <div class="topbar">
      <div>
        <h1>Programmatic Ads & SEO — Interactive MCQ Quiz</h1>
        <p class="lead">~62 mixed-difficulty questions on SEO, programmatic advertising, analytics, targeting and campaign metrics. Select an answer to get instant feedback. Use the buttons to reveal feedback for all, clear answers, or submit for scoring.</p>
      </div>
      <div style="min-width:280px;display:flex;align-items:center;">
        <div style="font-size:13px;color:var(--muted)">Progress</div>
        <div class="progress" aria-hidden><i id="prog"></i></div>
      </div>
    </div>

    <form id="quizForm" class="grid" autocomplete="off"></form>

    <div class="controls">
      <div style="display:flex;gap:8px">
        <button id="revealAll" type="button" class="secondary">Reveal Feedback for All</button>
        <button id="clearAll" type="button" class="secondary">Clear Answers</button>
      </div>
      <div style="display:flex;gap:8px">
        <button id="submitBtn" type="button">Submit Quiz</button>
      </div>
    </div>

    <div id="result"></div>
    <footer>Built from your notes. Tell me if you want this exported as a downloadable HTML file.</footer>
  </div>

<script>
const questions = [
  {q:'Ad "creatives" refers to:', opts:['Impressions','Publishers\' Ad space','Advertisers\' Ads','Both publisher and advertiser assets'], a:2, f:'Creatives are the ad materials produced by advertisers (visual, text, video).'},
  {q:'Ad Network usually operates on which side?', opts:['DSP','SSP','DMP','Search Engine'], a:1, f:'Ad networks aggregate publisher inventory and operate on the supply side with SSPs.'},
  {q:'Real-Time Bidding (RTB) is best described as:', opts:['Bidding on ad copies in real time','Bidding on ad creatives in real time','Bidding on creatives for a specific impression/ad space in real time','Bidding on keywords'], a:2, f:'RTB auctions occur per impression; creatives are served if the bid wins.'},
  {q:'SSP stands for:', opts:['Supply-Side Platform','Search Service Provider','Site-Side Proxy','Server-Side Processing'], a:0, f:'SSP is used by publishers to manage and sell ad inventory.'},
  {q:'DSP stands for:', opts:['Demand-Side Platform','Data Service Provider','Direct Sell Platform','Dynamic Supply Proxy'], a:0, f:'DSPs let advertisers buy inventory programmatically.'},
  {q:'DMP is primarily used for:', opts:['Serving creatives','Managing publisher inventory','Collecting and segmenting audience data','Real-time bidding'], a:2, f:'DMPs aggregate audience data from multiple sources for targeting.'},
  {q:'Ad Exchange is the:', opts:['Ad creative editor','Marketplace for real-time auctioning of inventory','Analytics dashboard','Canonical manager'], a:1, f:'Ad exchanges connect buyers and sellers and run RTB auctions.'},
  {q:'Retargeting audience means:', opts:['Targeting previous visitors to your site','Seeking lookalike audiences','Web searchers of similar products','All of the above'], a:0, f:'Retargeting specifically targets users who previously visited or engaged with your site.'},
  {q:'Tool to track internal traffic on a business site:', opts:['Google Ads','Google AdSense','Google Analytics','Google Search Console'], a:2, f:'Google Analytics tracks internal and external site traffic with filters.'},
  {q:'The <title> tag is important because:', opts:['It appears in SERP and influences clicks','It controls robots indexation','It is only visible on the page','It is a meta keyword'], a:0, f:'Title tag shows in SERP and is crucial for relevance and click-throughs.'},
  {q:'LSI (Latent Semantic Indexing) keywords are:', opts:['Exact keyword repeats only','Semantically related words to a topic','Robots directives','Ad exchange names'], a:1, f:'LSI keywords help search engines understand related concepts around a topic.'},
  {q:'LSA (Latent Semantic Analysis) is about:', opts:['Analyzing semantic connections and concept clusters','Creating ad creatives','Buying inventory','A canonical tag'], a:0, f:'LSA helps analyze semantically connected contexts and terms.'},
  {q:'Active-looking traffic (high commercial intent) typically comes from:', opts:['Social posts','Search queries for products','Random display impressions','Cold email lists'], a:1, f:'Search queries often carry purchase intent leading to higher conversion rates.'},
  {q:'Passive channels are best for:', opts:['Immediate conversions','Brand awareness and inspiration','Direct sales only','Indexing sitemaps'], a:1, f:'Passive channels like social media raise awareness rather than immediate conversions.'},
  {q:'CTR measures:', opts:['Clicks per Impressions','Impressions per Clicks','Revenue per Click','Orders per Impression'], a:0, f:'CTR = clicks ÷ impressions.'},
  {q:'FMV (Fair Market Value) means:', opts:['Lowest sale price','Price in an open market without coercion','Internal book value','Reserve auction price'], a:1, f:'FMV is what a willing buyer and seller would agree on freely.'},
  {q:'Display ads bought directly from publisher for premium placements is:', opts:['RTB','Direct Sale','Ad Exchange buying','DMP function'], a:1, f:'Direct sale involves negotiated guaranteed placements with publishers.'},
  {q:'Ad inventory refers to:', opts:['Publisher ad slots/pages','Advertiser budgets','Search keywords','Meta tags'], a:0, f:'Inventory is the available ad space publishers sell.'},
  {q:'Ad Server primarily:', opts:['Manages & serves creatives, tracks performance','Aggregates audience data','Runs RTB auctions','Creates sitemaps'], a:0, f:'Ad servers host creatives, deliver them, and record metrics like impressions and clicks.'},
  {q:'Syndicated data is:', opts:['Market data collected and sold by firms','Real-time bid logs','Creative assets','Robots meta outputs'], a:0, f:'Syndicated data is bought to augment targeting and audience insights.'},
  {q:'Omnichannel marketing means:', opts:['One-channel focus','Customer-centric cross-channel engagement','Only email marketing','SEO-only strategy'], a:1, f:'Omnichannel provides consistent experiences across customer preferred channels.'},
  {q:'Lookalike audience is:', opts:['A list of previous visitors','New users similar to seed customers','An SSP feature','A meta tag'], a:1, f:'Lookalikes find similar users to known high-value customers.'},
  {q:'Site retargeting delivers ads to:', opts:['Previous site visitors','Search engine users only','Only purchasers','Canonical URLs'], a:0, f:'It targets users who previously visited the website.'},
  {q:'Search retargeting uses:', opts:['Search behavior to target users','Only cookies','Sitemaps','Ad creatives'], a:0, f:'Search retargeting targets users based on search queries for similar products.'},
  {q:'Which is NOT a DMP function?', opts:['Compile audience data','Create segments','Buy inventory','Syndicate data'], a:2, f:'DMPs handle data for targeting; buying inventory is done via DSPs/Exchanges.'},
  {q:'Canonical tag helps to:', opts:['Mark preferred URL among duplicates','Hide pages from users','Increase CTR directly','Serve ads'], a:0, f:'Canonical tells search engines which URL to treat as the original to avoid duplicate issues.'},
  {q:'Robots.txt vs meta robots tag difference:', opts:['robots.txt is for images only','robots.txt blocks paths; meta robots controls per-page indexing','They are identical','robots meta controls sitemaps'], a:1, f:'robots.txt blocks crawler access at path-level; meta robots tag controls indexing/following per page.'},
  {q:'Meta description is:', opts:['Shown on the page body','Machine-readable in head and often used as SERP snippet','A link attribute','An ad creative'], a:1, f:'Meta descriptions are in the head and often displayed as search snippets.'},
  {q:'Good URL practice is to:', opts:['Use short descriptive permalinks with HTTPS','Include session IDs','Make them extremely long with dates','Use IP addresses'], a:0, f:'Short descriptive URLs with HTTPS are preferred for SEO and user trust.'},
  {q:'Utility pages to often noindex include:', opts:['Login, password reset, admin pages','Main product pages','Landing pages','Blog posts'], a:0, f:'Utility pages usually carry no SEO benefit and are often excluded from indexing.'},
  {q:'Anchor text "Click here" is:', opts:['Branded anchor','Naked link','Generic anchor text','Image alt text'], a:2, f:'"Click here" is generic and not SEO optimized.'},
  {q:'Alt attribute helps with:', opts:['Only page speed','Accessibility and image SEO','Buying ads','Blocking crawlers'], a:1, f:'Alt attributes describe images for accessibility and help search engines understand images.'},
  {q:'Sitemap XML helps:', opts:['List site hierarchy for crawlers','Replace navigation UI','Serve ads','Block indexing'], a:0, f:'XML sitemaps help crawlers discover and prioritize site pages.'},
  {q:'Deep linking means:', opts:['Linking only to home','Linking to specific internal pages beyond home','Blocking crawlers','Only external linking'], a:1, f:'Deep linking connects users and crawlers directly to internal content pages.'},
  {q:'Short-tail keywords are:', opts:['Broad general keywords with high volume','Specific long queries','Illegal keywords','Always low competition'], a:0, f:'Short-tail keywords are broad and competitive with high search volume.'},
  {q:'Long-tail keywords are:', opts:['Very generic','Specific niche queries with lower volume','Not useful','Only one word'], a:1, f:'Long-tail queries are specific and often have higher commercial intent.'},
  {q:'CPM stands for:', opts:['Cost Per Mille (thousand)','Cost Per Minute','Clicks Per Million','Creative Performance Metric'], a:0, f:'CPM is cost per thousand impressions.'},
  {q:'CPC stands for:', opts:['Cost Per Conversion','Cost Per Click','Clicks Per Campaign','Cost Per Customer'], a:1, f:'CPC is cost per click.'},
  {q:'Conversion rate roughly equals:', opts:['Clicks / impressions','Orders / clicks','Impressions / clicks','Avg session duration'], a:1, f:'Conversion rate normally measures conversions divided by clicks (or sessions depending on definition).'},
  {q:'UTM parameters are used to:', opts:['Block bots','Attribute traffic to campaigns in analytics','Serve ads','Change canonical URLs'], a:1, f:'UTMs help analytics identify traffic sources like campaign, medium, and source.'},
  {q:'Global site tag (gtag.js) is used to:', opts:['Manage robots.txt','Send events to Google Analytics/Ads','Serve sitemaps','Create meta tags'], a:1, f:'gtag.js collects event data and sends it to Google products for measurement.'},
  {q:'Google Ads is used by:', opts:['Publishers','Advertisers','SEO auditors','DMPs'], a:1, f:'Google Ads is the advertiser platform for running paid campaigns.'},
  {q:'Google AdSense is used by:', opts:['Advertisers','Publishers','Analysts','DMPs'], a:1, f:'AdSense allows publishers to monetize site inventory by showing ads.'},
  {q:'Google Search Console helps with:', opts:['Ad bidding','Monitoring indexing and search performance','Serving creatives','Managing SSPs'], a:1, f:'Search Console gives indexing and search query performance insights.'},
  {q:'DSPs/DSP tags place cookies or device IDs to:', opts:['Change canonical tags','Identify and retarget users','Improve meta descriptions','Generate sitemaps'], a:1, f:'Cookies/device IDs enable user identification for retargeting across sites.'},
  {q:'Retargeting lists commonly include:', opts:['Cart abandoners and product viewers','Only purchasers','Only searchers','Sitemaps'], a:0, f:'Lists are built from behaviors like product views or cart abandonment.'},
  {q:'Lower-funnel objectives target:', opts:['Top-of-funnel awareness only','Users close to purchase (product/cart pages)','Indexing issues','Canonical tags'], a:1, f:'Lower funnel targets high-intent users near conversion.'},
  {q:'Prospecting campaigns are aimed at:', opts:['Existing customers only','Finding new potential customers (lookalikes)','Robots.txt management','Ad server setup'], a:1, f:'Prospecting uses lookalikes and broad targeting to acquire new users.'},
  {q:'A/B testing in marketing is for:', opts:['Testing multiple asset versions to find best performer','Automatically increasing CTR','Buying inventory','Replacing analytics'], a:0, f:'A/B testing compares variants of creatives or pages to optimize performance.'},
  {q:'"Mad men" vs "Math men" refers to:', opts:['Creative ad era vs data-driven programmatic buying shift','SEO vs PPC','SSP vs DSP','Canonical vs meta tags'], a:0, f:'It describes the industry shift from intuition-driven to data-driven buying.'},
  {q:'Which is NOT on-page SEO?', opts:['Title tag','Meta description','Internal linking','AdSense configuration'], a:3, f:'AdSense is monetization and not an on-page SEO activity.'},
  {q:'Blended (universal) search results include:', opts:['Only blue organic links','Images, videos, maps and web results together','Only ads','Canonical listings'], a:1, f:'Blended search mixes different result types for queries.'},
  {q:'SILOing content structure means:', opts:['Random linking','Organizing related content into clusters and hierarchy','Hiding pages','Using only external links'], a:1, f:'SILO helps topical authority and site organization for SEO.'},
  {q:'Internal deep linking benefits:', opts:['Dilutes ranking','Helps crawlers discover deeper pages and distribute link equity','Increases page load','Removes meta tags'], a:1, f:'Deep links improve discoverability and help distribute authority.'},
  {q:'When should you use noindex?', opts:['Utility pages like login/reset','Main product pages','Important landing pages','Blog cornerstone content'], a:0, f:'Utility pages are often excluded from search to avoid low-value indexing.'},
  {q:'Naked link is:', opts:['A link showing the full URL as anchor text','A link without href','A hidden link','An image-only link'], a:0, f:'Naked link uses the raw URL as the clickable anchor text.'},
  {q:'Meta keywords tag today is:', opts:['Heavily used by Google','Mostly ignored by major search engines','Required for indexing','Used for robots control'], a:1, f:'Most search engines ignore meta keywords due to past abuse.'}
];

// render
const form = document.getElementById('quizForm');
questions.forEach((q,i)=>{
  const wrapper = document.createElement('div'); wrapper.className='question'; wrapper.id='q'+i;
  const qh = document.createElement('div'); qh.className='qhead'; qh.textContent=(i+1)+'. '+q.q; wrapper.appendChild(qh);
  const opts = document.createElement('div'); opts.className='opts';
  q.opts.forEach((o,j)=>{
    const id = `q_${i}_${j}`;
    const lab = document.createElement('label'); lab.className='opt'; lab.htmlFor=id;
    lab.innerHTML = `<input type='radio' name='q${i}' id='${id}' value='${j}' /> <span>${o}</span>`;
    opts.appendChild(lab);
  });
  wrapper.appendChild(opts);
  const fb = document.createElement('div'); fb.className='feedback'; fb.id='fb'+i; wrapper.appendChild(fb);
  form.appendChild(wrapper);
});

// instant feedback
form.addEventListener('change', e=>{
  const name = e.target.name; if(!name) return;
  if(!name.startsWith('q')) return;
  const qi = parseInt(name.replace('q',''),10);
  const val = parseInt(e.target.value,10);
  showFeedback(qi,val);
  updateProgress();
});

function showFeedback(i, val){
  const fb = document.getElementById('fb'+i);
  const q = questions[i];
  const right = q.opts[q.a];
  if(val===q.a){ fb.className='feedback show correct'; fb.innerHTML = '✅ Correct — '+q.f; }
  else { fb.className='feedback show incorrect'; fb.innerHTML = '❌ Incorrect — Correct answer: "'+right+'". '+q.f; }
}

function updateProgress(){
  const answered = document.querySelectorAll('input[type=radio]:checked').length;
  const pct = Math.round((answered/questions.length)*100);
  document.getElementById('prog').style.width = pct+'%';
}

// controls
document.getElementById('revealAll').addEventListener('click', ()=>{
  questions.forEach((q,i)=>{
    const sel = document.querySelector(`input[name=q${i}]:checked`);
    if(sel) showFeedback(i, parseInt(sel.value,10));
    else { const fb=document.getElementById('fb'+i); fb.className='feedback show incorrect'; fb.innerHTML='⚠️ No answer selected — Correct: "'+q.opts[q.a]+'". '+q.f; }
  });
  updateProgress();
});

document.getElementById('clearAll').addEventListener('click', ()=>{
  document.querySelectorAll('input[type=radio]').forEach(inp=>inp.checked=false);
  document.querySelectorAll('.feedback').forEach(f=>{f.className='feedback'; f.innerHTML='';});
  document.getElementById('prog').style.width='0%'; document.getElementById('result').innerHTML='';
});

document.getElementById('submitBtn').addEventListener('click', ()=>{
  let correct=0; let answered=0;
  questions.forEach((q,i)=>{
    const sel = document.querySelector(`input[name=q${i}]:checked`);
    if(sel){ answered++; if(parseInt(sel.value,10)===q.a) correct++; }
    else { const fb=document.getElementById('fb'+i); fb.className='feedback show incorrect'; fb.innerHTML='⚠️ No answer selected — Correct: "'+q.opts[q.a]+'". '+q.f; }
  });
  const pct = Math.round((correct/questions.length)*100);
  document.getElementById('result').innerHTML = `<div><strong>Score:</strong> ${correct} / ${questions.length} (${pct}%) — Answered ${answered} questions.</div>`;
  document.getElementById('prog').style.width = pct+'%';
  window.scrollTo({top:document.body.scrollHeight,behavior:'smooth'});
});

</script>
</body>
</html>
