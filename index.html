<html lang="en" >
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Dklinity - Clinical Trials Database with ARM & References</title>
  <script src="https://cdn.tailwindcss.com"></script>
  <link
    rel="stylesheet"
    href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css"
  />
  <link
    href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600&display=swap"
    rel="stylesheet"
  />
  <style>
    body {
      font-family: 'Inter', sans-serif;
    }
    .scrollbar-thin::-webkit-scrollbar {
      width: 6px;
      height: 6px;
    }
    .scrollbar-thin::-webkit-scrollbar-thumb {
      background-color: rgba(107, 114, 128, 0.5);
      border-radius: 3px;
    }
    /* Simple contenteditable styling */
    .editable-table {
      border: 1px solid #cbd5e1;
      border-radius: 0.375rem;
      padding: 0.5rem;
      min-height: 100px;
      overflow: auto;
      background-color: #f9fafb;
    }
  </style>
</head>
<body class="bg-gray-50 min-h-screen flex flex-col">

  <!-- Login Overlay -->
  <div id="loginOverlay" class="fixed inset-0 bg-gray-900 bg-opacity-80 flex items-center justify-center z-50">
    <div class="bg-white rounded-lg shadow-lg p-8 w-full max-w-md">
      <h2 class="text-2xl font-semibold mb-6 text-center text-blue-900">Login to Dklinity</h2>
      <form id="loginForm" class="space-y-4" autocomplete="off" novalidate>
        <div>
          <label for="username" class="block font-medium mb-1">Username</label>
          <input type="text" id="username" name="username" required autocomplete="username" class="w-full border border-gray-300 rounded px-3 py-2 focus:outline-none focus:ring-2 focus:ring-blue-600" />
        </div>
        <div>
          <label for="password" class="block font-medium mb-1">Password</label>
          <input type="password" id="password" name="password" required autocomplete="current-password" class="w-full border border-gray-300 rounded px-3 py-2 focus:outline-none focus:ring-2 focus:ring-blue-600" />
        </div>
        <div id="loginMessage" class="text-sm text-red-600 min-h-[1.25rem]"></div>
        <button type="submit" class="w-full bg-blue-900 text-white font-semibold rounded px-4 py-2 hover:bg-blue-800 transition">
          <i class="fas fa-sign-in-alt mr-2"></i> Login
        </button>
      </form>
    </div>
  </div>

  <div id="appContent" class="hidden flex flex-col min-h-screen">
    <header class="bg-blue-900 text-white shadow">
      <div class="container mx-auto px-4 py-4 flex flex-col md:flex-row md:items-center md:justify-between">
        <h1 class="text-2xl font-semibold flex items-center gap-2">
          <i class="fas fa-database"></i> Dklinity
        </h1>
        <nav class="mt-3 md:mt-0">
          <ul class="flex flex-wrap gap-4 text-sm md:text-base">
            <li><a href="#search" class="hover:underline">Search Trials</a></li>
            <li><a href="#add-trial" class="hover:underline">Add New Trial</a></li>
          </ul>
        </nav>
      </div>
    </header>

    <main class="container mx-auto px-4 py-6 flex-grow">
      <!-- Trial Search Section -->
      <section id="search" class="mb-12">
        <h2 class="text-3xl font-semibold mb-4 text-blue-900 flex items-center gap-3">
          <i class="fas fa-search"></i> Search Trials
        </h2>
        <form id="trialSearchForm" class="bg-white p-6 rounded-lg shadow-md grid grid-cols-1 md:grid-cols-4 gap-6">
          <div class="md:col-span-2">
            <label for="searchTrialId" class="block font-medium mb-1">Trial ID</label>
            <input type="text" id="searchTrialId" name="trial_id" placeholder="e.g. ABC123 or 1" class="w-full border border-gray-300 rounded px-3 py-2 focus:outline-none focus:ring-2 focus:ring-blue-600" />
          </div>
          <div class="md:col-span-2">
            <label class="block font-medium mb-1">Other Study ID(s)</label>
            <div id="searchOtherStudyIdsContainer" class="space-y-2">
              <input type="text" name="other_study_id" placeholder="Other Study ID" class="w-full border border-gray-300 rounded px-3 py-2 focus:outline-none focus:ring-2 focus:ring-blue-600" />
            </div>
            <button type="button" id="addSearchOtherStudyIdBtn" class="mt-2 text-blue-700 hover:underline text-sm flex items-center gap-1">
              <i class="fas fa-plus"></i> Add another Other Study ID
            </button>
          </div>
          <div class="md:col-span-2">
            <label class="block font-medium mb-1">Indication(s)</label>
            <div id="searchIndicationsContainer" class="space-y-2">
              <input type="text" name="indication" placeholder="Indication" class="w-full border border-gray-300 rounded px-3 py-2 focus:outline-none focus:ring-2 focus:ring-blue-600" />
            </div>
            <button type="button" id="addSearchIndicationBtn" class="mt-2 text-blue-700 hover:underline text-sm flex items-center gap-1">
              <i class="fas fa-plus"></i> Add another Indication
            </button>
          </div>
          <div>
            <label for="searchTitle" class="block font-medium mb-1">Title</label>
            <input type="text" id="searchTitle" name="title" placeholder="Trial title keywords" class="w-full border border-gray-300 rounded px-3 py-2 focus:outline-none focus:ring-2 focus:ring-blue-600" />
          </div>
          <div>
            <label for="searchPhase" class="block font-medium mb-1">Phase</label>
            <select id="searchPhase" name="phase" class="w-full border border-gray-300 rounded px-3 py-2 focus:outline-none focus:ring-2 focus:ring-blue-600">
              <option value="">Any</option>
              <option value="Phase 1">Phase 1</option>
              <option value="Phase 2">Phase 2</option>
              <option value="Phase 3">Phase 3</option>
              <option value="Phase 4">Phase 4</option>
            </select>
          </div>
          <div>
            <label for="searchStatus" class="block font-medium mb-1">Status</label>
            <select id="searchStatus" name="status" class="w-full border border-gray-300 rounded px-3 py-2 focus:outline-none focus:ring-2 focus:ring-blue-600">
              <option value="">Any</option>
              <option value="Recruiting">Recruiting</option>
              <option value="Active">Active</option>
              <option value="Completed">Completed</option>
              <option value="Terminated">Terminated</option>
              <option value="Suspended">Suspended</option>
            </select>
          </div>
          <div class="flex items-end">
            <button type="submit" class="w-full bg-blue-900 text-white font-semibold rounded px-4 py-2 hover:bg-blue-800 transition">
              <i class="fas fa-search mr-2"></i> Search
            </button>
          </div>
        </form>
        <div id="searchResults" class="mt-8 bg-white rounded-lg shadow p-6 min-h-[150px]">
          <p class="text-gray-600 italic">No search performed yet.</p>
        </div>
      </section>

      <!-- Add Trial Section -->
      <section id="add-trial" class="mb-12">
        <h2 class="text-3xl font-semibold mb-4 text-blue-900 flex items-center gap-3">
          <i class="fas fa-plus-circle"></i> Add New Trial
        </h2>
        <form id="addTrialForm" class="bg-white p-6 rounded-lg shadow-md grid grid-cols-1 md:grid-cols-2 gap-6 max-w-3xl">
          <div class="md:col-span-2">
            <label for="trialId" class="block font-medium mb-1">Trial ID *</label>
            <input type="text" id="trialId" name="trial_id" required placeholder="Unique Trial ID (can include letters and numbers)" class="w-full border border-gray-300 rounded px-3 py-2 focus:outline-none focus:ring-2 focus:ring-blue-600" />
          </div>
          <div class="md:col-span-2">
            <label class="block font-medium mb-1">Other Study ID(s)</label>
            <div id="addOtherStudyIdsContainer" class="space-y-2">
              <input type="text" name="other_study_id" placeholder="Other Study ID" class="w-full border border-gray-300 rounded px-3 py-2 focus:outline-none focus:ring-2 focus:ring-blue-600" />
            </div>
            <button type="button" id="addOtherStudyIdBtn" class="mt-2 text-blue-700 hover:underline text-sm flex items-center gap-1">
              <i class="fas fa-plus"></i> Add another Other Study ID
            </button>
          </div>
          <div class="md:col-span-2">
            <label class="block font-medium mb-1">Indication(s)</label>
            <div id="addIndicationsContainer" class="space-y-2">
              <input type="text" name="indication" placeholder="Indication" class="w-full border border-gray-300 rounded px-3 py-2 focus:outline-none focus:ring-2 focus:ring-blue-600" />
            </div>
            <button type="button" id="addIndicationBtn" class="mt-2 text-blue-700 hover:underline text-sm flex items-center gap-1">
              <i class="fas fa-plus"></i> Add another Indication
            </button>
          </div>
          <div>
            <label for="trialTitle" class="block font-medium mb-1">Title *</label>
            <input type="text" id="trialTitle" name="title" required placeholder="Trial title" class="w-full border border-gray-300 rounded px-3 py-2 focus:outline-none focus:ring-2 focus:ring-blue-600" />
          </div>
          <div>
            <label for="trialEnrollment" class="block font-medium mb-1">Enrollment</label>
            <input type="number" id="trialEnrollment" name="enrollment" min="0" placeholder="Number of participants" class="w-full border border-gray-300 rounded px-3 py-2 focus:outline-none focus:ring-2 focus:ring-blue-600" />
          </div>
          <div>
            <label for="trialPhase" class="block font-medium mb-1">Phase</label>
            <select id="trialPhase" name="phase" class="w-full border border-gray-300 rounded px-3 py-2 focus:outline-none focus:ring-2 focus:ring-blue-600">
              <option value="">Select phase</option>
              <option value="Phase 1">Phase 1</option>
              <option value="Phase 2">Phase 2</option>
              <option value="Phase 3">Phase 3</option>
              <option value="Phase 4">Phase 4</option>
            </select>
          </div>
          <div>
            <label for="trialStudyType" class="block font-medium mb-1">Study Type</label>
            <select id="trialStudyType" name="study_type" class="w-full border border-gray-300 rounded px-3 py-2 focus:outline-none focus:ring-2 focus:ring-blue-600">
              <option value="">Select study type</option>
              <option value="Interventional">Interventional</option>
              <option value="Observational">Observational</option>
              <option value="Expanded Access">Expanded Access</option>
              <option value="Other">Other</option>
            </select>
          </div>
          <div>
            <label for="trialStatus" class="block font-medium mb-1">Status</label>
            <select id="trialStatus" name="status" class="w-full border border-gray-300 rounded px-3 py-2 focus:outline-none focus:ring-2 focus:ring-blue-600">
              <option value="">Select status</option>
              <option value="Recruiting">Recruiting</option>
              <option value="Active">Active</option>
              <option value="Completed">Completed</option>
              <option value="Terminated">Terminated</option>
              <option value="Suspended">Suspended</option>
            </select>
          </div>
          <div>
            <label for="trialSponsor" class="block font-medium mb-1">Sponsor</label>
            <input type="text" id="trialSponsor" name="sponsor" placeholder="Sponsor company name" class="w-full border border-gray-300 rounded px-3 py-2 focus:outline-none focus:ring-2 focus:ring-blue-600" />
          </div>
          <div class="md:col-span-2">
            <label class="block font-medium mb-1">Product Tags</label>
            <div id="productTagsContainer" class="space-y-2">
              <input type="text" name="product_tag" placeholder="Product name" class="w-full border border-gray-300 rounded px-3 py-2 focus:outline-none focus:ring-2 focus:ring-blue-600" />
            </div>
            <button type="button" id="addProductTagBtn" class="mt-2 text-blue-700 hover:underline text-sm flex items-center gap-1">
              <i class="fas fa-plus"></i> Add another Product
            </button>
          </div>
          <div>
            <label for="trialAllocation" class="block font-medium mb-1">Allocation</label>
            <select id="trialAllocation" name="allocation" class="w-full border border-gray-300 rounded px-3 py-2 focus:outline-none focus:ring-2 focus:ring-blue-600">
              <option value="">Select allocation</option>
              <option value="Randomized">Randomized</option>
              <option value="Non-Randomized">Non-Randomized</option>
              <option value="Other">Other</option>
            </select>
          </div>
          <div>
            <label for="trialStartDate" class="block font-medium mb-1">Start Date</label>
            <input type="date" id="trialStartDate" name="start_date" class="w-full border border-gray-300 rounded px-3 py-2 focus:outline-none focus:ring-2 focus:ring-blue-600" />
          </div>
          <div>
            <label for="trialEndDate" class="block font-medium mb-1">End Date</label>
            <input type="date" id="trialEndDate" name="end_date" class="w-full border border-gray-300 rounded px-3 py-2 focus:outline-none focus:ring-2 focus:ring-blue-600" />
          </div>
          <div class="md:col-span-2 flex justify-end gap-4">
            <button type="reset" class="bg-gray-400 text-white font-semibold rounded px-6 py-2 hover:bg-gray-500 transition">
              Reset
            </button>
            <button type="submit" class="bg-green-700 text-white font-semibold rounded px-6 py-2 hover:bg-green-600 transition">
              <i class="fas fa-save mr-2"></i> Add Trial
            </button>
          </div>
        </form>
        <div id="addTrialMessage" class="mt-4 text-sm"></div>
      </section>

      <!-- Trial Details & Tabs Section (hidden initially) -->
      <section id="trialDetailsSection" class="hidden bg-white rounded-lg shadow-md p-6 max-w-7xl mx-auto">
        <div class="flex justify-between items-center mb-4">
          <h2 id="trialDetailsTitle" class="text-3xl font-semibold text-blue-900 flex items-center gap-3">
            <i class="fas fa-vials"></i> Trial Details
          </h2>
          <button id="closeTrialDetailsBtn" aria-label="Close trial details" class="text-gray-600 hover:text-gray-900 text-2xl font-bold">&times;</button>
        </div>

        <div id="trialSummary" class="mb-6 border border-gray-300 rounded p-4 bg-gray-50 grid grid-cols-1 md:grid-cols-3 gap-4 text-gray-700">
        </div>

        <nav class="mb-6 border-b border-gray-300">
          <ul id="tabs" class="flex flex-wrap gap-2 text-sm font-semibold text-gray-600">
            <li><button data-tab="products" class="tab-btn px-4 py-2 rounded-t border border-b-0 border-gray-300 bg-gray-200 text-blue-900">Products (ARM-wise)</button></li>
            <li><button data-tab="patients" class="tab-btn px-4 py-2 rounded-t border border-b-0 border-gray-300 hover:bg-gray-100">Patients (ARM-wise)</button></li>
            <li><button data-tab="adverseEvents" class="tab-btn px-4 py-2 rounded-t border border-b-0 border-gray-300 hover:bg-gray-100">Adverse Events (ARM-wise)</button></li>
            <li><button data-tab="responseData" class="tab-btn px-4 py-2 rounded-t border border-b-0 border-gray-300 hover:bg-gray-100">Response Data</button></li>
            <li><button data-tab="survivalData" class="tab-btn px-4 py-2 rounded-t border border-b-0 border-gray-300 hover:bg-gray-100">Survival Data</button></li>
            <li><button data-tab="regulatoryEvents" class="tab-btn px-4 py-2 rounded-t border border-b-0 border-gray-300 hover:bg-gray-100">Regulatory Announcements</button></li>
            <li><button data-tab="references" class="tab-btn px-4 py-2 rounded-t border border-b-0 border-gray-300 hover:bg-gray-100">All References</button></li>
          </ul>
        </nav>

        <div id="tabContent" class="min-h-[400px]"></div>
      </section>
    </main>

    <footer class="bg-blue-900 text-white py-4 text-center text-sm">
      Dklinity &copy; 2024 Clinical Trials Database
    </footer>
  </div>

  <script>
    // In-memory data storage simulation
    const trials = [];
    const products = [];
    const patients = [];
    const adverseEvents = [];
    const responseData = [];
    const survivalData = [];
    const regulatoryEvents = [];
    const references = []; // unified references for all tabs
    const trial_products = [];

    // Login credentials
    const validUsername = 'Dilip';
    const validPassword = 'Dilip@321';

    // Show login overlay initially
    const loginOverlay = document.getElementById('loginOverlay');
    const appContent = document.getElementById('appContent');
    const loginForm = document.getElementById('loginForm');
    const loginMessage = document.getElementById('loginMessage');

    loginForm.addEventListener('submit', e => {
      e.preventDefault();
      const username = loginForm.username.value.trim();
      const password = loginForm.password.value;

      if (username === validUsername && password === validPassword) {
        loginOverlay.classList.add('hidden');
        appContent.classList.remove('hidden');
        loginForm.reset();
        loginMessage.textContent = '';
      } else {
        loginMessage.textContent = 'Invalid username or password.';
      }
    });

    function generateId(collection) {
      return collection.length ? collection[collection.length - 1].id + 1 : 1;
    }

    function showMessage(elementId, message, isError = false) {
      const el = document.getElementById(elementId);
      el.textContent = message;
      el.className = isError ? 'mt-4 text-sm text-red-600' : 'mt-4 text-sm text-green-600';
      setTimeout(() => {
        el.textContent = '';
      }, 5000);
    }

    // Add Other Study ID input fields dynamically (Add Trial Form)
    const addOtherStudyIdBtn = document.getElementById('addOtherStudyIdBtn');
    const addOtherStudyIdsContainer = document.getElementById('addOtherStudyIdsContainer');
    addOtherStudyIdBtn.addEventListener('click', () => {
      const input = document.createElement('input');
      input.type = 'text';
      input.name = 'other_study_id';
      input.placeholder = 'Other Study ID';
      input.className = 'w-full border border-gray-300 rounded px-3 py-2 focus:outline-none focus:ring-2 focus:ring-blue-600';
      addOtherStudyIdsContainer.appendChild(input);
    });

    // Add Indication input fields dynamically (Add Trial Form)
    const addIndicationBtn = document.getElementById('addIndicationBtn');
    const addIndicationsContainer = document.getElementById('addIndicationsContainer');
    addIndicationBtn.addEventListener('click', () => {
      const input = document.createElement('input');
      input.type = 'text';
      input.name = 'indication';
      input.placeholder = 'Indication';
      input.className = 'w-full border border-gray-300 rounded px-3 py-2 focus:outline-none focus:ring-2 focus:ring-blue-600';
      addIndicationsContainer.appendChild(input);
    });

    // Add Other Study ID input fields dynamically (Search Form)
    const addSearchOtherStudyIdBtn = document.getElementById('addSearchOtherStudyIdBtn');
    const searchOtherStudyIdsContainer = document.getElementById('searchOtherStudyIdsContainer');
    addSearchOtherStudyIdBtn.addEventListener('click', () => {
      const input = document.createElement('input');
      input.type = 'text';
      input.name = 'other_study_id';
      input.placeholder = 'Other Study ID';
      input.className = 'w-full border border-gray-300 rounded px-3 py-2 focus:outline-none focus:ring-2 focus:ring-blue-600';
      searchOtherStudyIdsContainer.appendChild(input);
    });

    // Add Indication input fields dynamically (Search Form)
    const addSearchIndicationBtn = document.getElementById('addSearchIndicationBtn');
    const searchIndicationsContainer = document.getElementById('searchIndicationsContainer');
    addSearchIndicationBtn.addEventListener('click', () => {
      const input = document.createElement('input');
      input.type = 'text';
      input.name = 'indication';
      input.placeholder = 'Indication';
      input.className = 'w-full border border-gray-300 rounded px-3 py-2 focus:outline-none focus:ring-2 focus:ring-blue-600';
      searchIndicationsContainer.appendChild(input);
    });

    // Add Product Tag input fields dynamically (Add Trial Form)
    const addProductTagBtn = document.getElementById('addProductTagBtn');
    const productTagsContainer = document.getElementById('productTagsContainer');
    addProductTagBtn.addEventListener('click', () => {
      const input = document.createElement('input');
      input.type = 'text';
      input.name = 'product_tag';
      input.placeholder = 'Product name';
      input.className = 'w-full border border-gray-300 rounded px-3 py-2 focus:outline-none focus:ring-2 focus:ring-blue-600';
      productTagsContainer.appendChild(input);
    });

    // Add Trial Form Submission
    document.getElementById('addTrialForm').addEventListener('submit', function (e) {
      e.preventDefault();
      const formData = new FormData(this);
      const trial_id = formData.get('trial_id').trim();
      if (!trial_id) {
        showMessage('addTrialMessage', 'Trial ID is required.', true);
        return;
      }
      // Check for duplicate trial_id
      if (trials.some(t => t.id === trial_id)) {
        showMessage('addTrialMessage', `Trial ID "${trial_id}" already exists. Please use a unique Trial ID.`, true);
        return;
      }
      const title = formData.get('title').trim();
      if (!title) {
        showMessage('addTrialMessage', 'Title is required.', true);
        return;
      }
      // Collect multiple other_study_id inputs
      const other_study_ids = [];
      this.querySelectorAll('input[name="other_study_id"]').forEach(input => {
        const val = input.value.trim();
        if (val) other_study_ids.push(val);
      });
      // Collect multiple indications inputs
      const indications = [];
      this.querySelectorAll('input[name="indication"]').forEach(input => {
        const val = input.value.trim();
        if (val) indications.push(val);
      });
      const enrollmentRaw = formData.get('enrollment');
      const enrollment = enrollmentRaw ? parseInt(enrollmentRaw) : null;
      const phase = formData.get('phase');
      const study_type = formData.get('study_type') || null;
      const status = formData.get('status');
      const sponsor = formData.get('sponsor').trim() || null;
      // Collect multiple product_tag inputs
      const product_tags = [];
      this.querySelectorAll('input[name="product_tag"]').forEach(input => {
        const val = input.value.trim();
        if (val) product_tags.push(val);
      });

      const allocation = formData.get('allocation') || null;
      const start_date = formData.get('start_date') || null;
      const end_date = formData.get('end_date') || null;

      const newTrial = {
        id: trial_id,
        title,
        other_study_id: other_study_ids.length ? other_study_ids : null,
        indication: indications.length ? indications : null,
        enrollment,
        phase: phase || null,
        study_type,
        status: status || null,
        sponsor,
        product_tags,
        allocation,
        start_date,
        end_date,
        created_at: new Date().toISOString()
      };
      trials.push(newTrial);
      this.reset();
      // Reset dynamic inputs to one input each
      addOtherStudyIdsContainer.innerHTML = '';
      const firstOtherStudyInput = document.createElement('input');
      firstOtherStudyInput.type = 'text';
      firstOtherStudyInput.name = 'other_study_id';
      firstOtherStudyInput.placeholder = 'Other Study ID';
      firstOtherStudyInput.className = 'w-full border border-gray-300 rounded px-3 py-2 focus:outline-none focus:ring-2 focus:ring-blue-600';
      addOtherStudyIdsContainer.appendChild(firstOtherStudyInput);

      addIndicationsContainer.innerHTML = '';
      const firstIndicationInput = document.createElement('input');
      firstIndicationInput.type = 'text';
      firstIndicationInput.name = 'indication';
      firstIndicationInput.placeholder = 'Indication';
      firstIndicationInput.className = 'w-full border border-gray-300 rounded px-3 py-2 focus:outline-none focus:ring-2 focus:ring-blue-600';
      addIndicationsContainer.appendChild(firstIndicationInput);

      productTagsContainer.innerHTML = '';
      const firstProductTagInput = document.createElement('input');
      firstProductTagInput.type = 'text';
      firstProductTagInput.name = 'product_tag';
      firstProductTagInput.placeholder = 'Product name';
      firstProductTagInput.className = 'w-full border border-gray-300 rounded px-3 py-2 focus:outline-none focus:ring-2 focus:ring-blue-600';
      productTagsContainer.appendChild(firstProductTagInput);

      showMessage('addTrialMessage', `Trial ID "${newTrial.id}" added successfully.`);

      loadTrialDetails(newTrial.id);
      document.getElementById('trialDetailsSection').scrollIntoView({ behavior: 'smooth' });
    });

    // Search Trials
    document.getElementById('trialSearchForm').addEventListener('submit', function (e) {
      e.preventDefault();
      const formData = new FormData(this);
      const trialId = formData.get('trial_id').trim().toLowerCase();

      // Collect multiple other_study_id inputs
      const otherStudyIds = [];
      this.querySelectorAll('input[name="other_study_id"]').forEach(input => {
        const val = input.value.trim().toLowerCase();
        if (val) otherStudyIds.push(val);
      });

      // Collect multiple indications inputs
      const indications = [];
      this.querySelectorAll('input[name="indication"]').forEach(input => {
        const val = input.value.trim().toLowerCase();
        if (val) indications.push(val);
      });

      const title = formData.get('title').trim().toLowerCase();
      const phase = formData.get('phase');
      const status = formData.get('status');

      let results = trials.filter(trial => {
        // Trial ID match (case insensitive)
        const trialIdMatch = trialId === '' || (trial.id && trial.id.toLowerCase().includes(trialId));
        // Other Study ID match: any of the entered otherStudyIds matches any in trial.other_study_id array (case insensitive)
        let otherStudyIdMatch = true;
        if (otherStudyIds.length > 0) {
          if (!trial.other_study_id || !Array.isArray(trial.other_study_id)) {
            otherStudyIdMatch = false;
          } else {
            otherStudyIdMatch = otherStudyIds.some(osid => trial.other_study_id.some(tosid => tosid.toLowerCase() === osid));
          }
        }
        // Indication match: any of the entered indications matches any in trial.indication array (case insensitive)
        let indicationMatch = true;
        if (indications.length > 0) {
          if (!trial.indication || !Array.isArray(trial.indication)) {
            indicationMatch = false;
          } else {
            indicationMatch = indications.some(ind => trial.indication.some(tind => tind.toLowerCase().includes(ind)));
          }
        }
        // Title match
        const titleMatch = title === '' || (trial.title && trial.title.toLowerCase().includes(title));
        // Phase match
        const phaseMatch = phase === '' || trial.phase === phase;
        // Status match
        const statusMatch = status === '' || trial.status === status;

        return trialIdMatch && otherStudyIdMatch && indicationMatch && titleMatch && phaseMatch && statusMatch;
      });

      const resultsContainer = document.getElementById('searchResults');
      if (results.length === 0) {
        resultsContainer.innerHTML = '<p class="text-gray-600 italic">No trials found matching the criteria.</p>';
        return;
      }

      let html = `<div class="overflow-x-auto">
        <table class="min-w-full border border-gray-300 rounded-md">
          <thead class="bg-blue-900 text-white">
            <tr>
              <th class="px-4 py-2 text-left">Trial ID</th>
              <th class="px-4 py-2 text-left">Other Study ID(s)</th>
              <th class="px-4 py-2 text-left">Title</th>
              <th class="px-4 py-2 text-left">Indication(s)</th>
              <th class="px-4 py-2 text-left">Enrollment</th>
              <th class="px-4 py-2 text-left">Phase</th>
              <th class="px-4 py-2 text-left">Study Type</th>
              <th class="px-4 py-2 text-left">Status</th>
              <th class="px-4 py-2 text-left">Sponsor</th>
              <th class="px-4 py-2 text-left">Product Tags</th>
              <th class="px-4 py-2 text-left">Allocation</th>
              <th class="px-4 py-2 text-left">Start Date</th>
              <th class="px-4 py-2 text-left">End Date</th>
              <th class="px-4 py-2 text-left">Actions</th>
            </tr>
          </thead>
          <tbody>`;

      for (const trial of results) {
        html += `<tr class="border-t border-gray-200 hover:bg-gray-100" tabindex="0" aria-label="View or edit trial ${trial.id}">
          <td class="px-4 py-2">${trial.id}</td>
          <td class="px-4 py-2">${trial.other_study_id && Array.isArray(trial.other_study_id) ? trial.other_study_id.join(', ') : ''}</td>
          <td class="px-4 py-2">${trial.title}</td>
          <td class="px-4 py-2">${trial.indication && Array.isArray(trial.indication) ? trial.indication.join(', ') : ''}</td>
          <td class="px-4 py-2">${trial.enrollment !== null && trial.enrollment !== undefined ? trial.enrollment : ''}</td>
          <td class="px-4 py-2">${trial.phase || ''}</td>
          <td class="px-4 py-2">${trial.study_type || ''}</td>
          <td class="px-4 py-2">${trial.status || ''}</td>
          <td class="px-4 py-2">${trial.sponsor || ''}</td>
          <td class="px-4 py-2">${trial.product_tags && trial.product_tags.length ? trial.product_tags.join(', ') : ''}</td>
          <td class="px-4 py-2">${trial.allocation || ''}</td>
          <td class="px-4 py-2">${trial.start_date || ''}</td>
          <td class="px-4 py-2">${trial.end_date || ''}</td>
          <td class="px-4 py-2">
            <button data-trial-id="${trial.id}" class="view-edit-btn bg-blue-700 text-white px-3 py-1 rounded hover:bg-blue-600 transition text-sm">
              <i class="fas fa-edit"></i> Edit
            </button>
          </td>
        </tr>`;
      }

      html += `</tbody></table></div>`;

      resultsContainer.innerHTML = html;

      const editButtons = resultsContainer.querySelectorAll('.view-edit-btn');
      editButtons.forEach(btn => {
        btn.addEventListener('click', () => {
          const trialId = btn.getAttribute('data-trial-id');
          loadTrialDetails(trialId);
          document.getElementById('trialDetailsSection').scrollIntoView({ behavior: 'smooth' });
        });
      });
    });

    let currentTrialId = null;

    function loadTrialDetails(trialId) {
      const trial = trials.find(t => t.id === trialId);
      if (!trial) return;

      const detailsSection = document.getElementById('trialDetailsSection');
      detailsSection.classList.remove('hidden');

      const summary = `
        <div><strong>Trial ID:</strong> ${trial.id}</div>
        <div><strong>Other Study ID(s):</strong> ${trial.other_study_id && Array.isArray(trial.other_study_id) ? trial.other_study_id.join(', ') : 'N/A'}</div>
        <div><strong>Title:</strong> ${trial.title}</div>
        <div><strong>Indication(s):</strong> ${trial.indication && Array.isArray(trial.indication) ? trial.indication.join(', ') : 'N/A'}</div>
        <div><strong>Enrollment:</strong> ${trial.enrollment !== null && trial.enrollment !== undefined ? trial.enrollment : 'N/A'}</div>
        <div><strong>Phase:</strong> ${trial.phase || 'N/A'}</div>
        <div><strong>Study Type:</strong> ${trial.study_type || 'N/A'}</div>
        <div><strong>Status:</strong> ${trial.status || 'N/A'}</div>
        <div><strong>Sponsor:</strong> ${trial.sponsor || 'N/A'}</div>
        <div><strong>Product Tags:</strong> ${trial.product_tags && trial.product_tags.length ? trial.product_tags.join(', ') : 'N/A'}</div>
        <div><strong>Allocation:</strong> ${trial.allocation || 'N/A'}</div>
        <div><strong>Start Date:</strong> ${trial.start_date || 'N/A'}</div>
        <div><strong>End Date:</strong> ${trial.end_date || 'N/A'}</div>
        <div><strong>Created At:</strong> ${new Date(trial.created_at).toLocaleString()}</div>
      `;
      document.getElementById('trialSummary').innerHTML = summary;

      currentTrialId = trialId;

      const tabButtons = document.querySelectorAll('.tab-btn');
      tabButtons.forEach(btn => {
        btn.classList.remove('bg-gray-200', 'text-blue-900');
        btn.classList.add('hover:bg-gray-100');
      });
      tabButtons[0].classList.add('bg-gray-200', 'text-blue-900');
      loadTabContent('products');

      resetAllTabForms();
    }

    document.getElementById('closeTrialDetailsBtn').addEventListener('click', () => {
      document.getElementById('trialDetailsSection').classList.add('hidden');
      currentTrialId = null;
    });

    document.getElementById('tabs').addEventListener('click', e => {
      if (!e.target.classList.contains('tab-btn')) return;
      const tab = e.target.getAttribute('data-tab');
      if (!tab) return;

      const tabButtons = document.querySelectorAll('.tab-btn');
      tabButtons.forEach(btn => {
        btn.classList.remove('bg-gray-200', 'text-blue-900');
        btn.classList.add('hover:bg-gray-100');
      });
      e.target.classList.add('bg-gray-200', 'text-blue-900');

      loadTabContent(tab);
    });

    function resetAllTabForms() {
      const forms = document.querySelectorAll('#tabContent form');
      forms.forEach(f => f.reset());
    }

    // === ARM management ===
    // For simplicity, arms are stored as array of strings per trial
    // We'll allow user to add arms in product tab and reuse in other tabs

    // Store arms per trial: { trialId: [armName1, armName2, ...] }
    const trialArms = {};

    // Get arms for current trial or empty array
    function getArms(trialId) {
      if (!trialArms[trialId]) trialArms[trialId] = [];
      return trialArms[trialId];
    }

    // Add arm if not exists
    function addArm(trialId, armName) {
      if (!trialArms[trialId]) trialArms[trialId] = [];
      if (!trialArms[trialId].includes(armName)) trialArms[trialId].push(armName);
    }

    // === References management ===
    // references: { id, trial_id, tab, source_name, link }
    // We'll add references from all tabs here and show in References tab

    // Add reference helper
    function addReference(trialId, tab, source_name, link) {
      if (!source_name || !link) return;
      // Check duplicate
      if (references.some(r => r.trial_id === trialId && r.tab === tab && r.source_name === source_name && r.link === link)) return;
      references.push({
        id: generateId(references),
        trial_id: trialId,
        tab,
        source_name,
        link
      });
    }

    // Load tab content dispatcher
    function loadTabContent(tab) {
      if (!currentTrialId) return;
      const container = document.getElementById('tabContent');
      container.innerHTML = '';

      switch (tab) {
        case 'products': renderProductsTab(container, currentTrialId); break;
        case 'patients': renderPatientsTab(container, currentTrialId); break;
        case 'adverseEvents': renderAdverseEventsTab(container, currentTrialId); break;
        case 'responseData': renderResponseDataTab(container, currentTrialId); break;
        case 'survivalData': renderSurvivalDataTab(container, currentTrialId); break;
        case 'regulatoryEvents': renderRegulatoryEventsTab(container, currentTrialId); break;
        case 'references': renderReferencesTab(container, currentTrialId); break;
        default: container.innerHTML = `<p class="text-gray-600 italic">Tab "${tab}" content not implemented.</p>`;
      }
    }

    // === PRODUCTS TAB ===
    // ARM wise product addition with dose and dosage details
    // Product Name is free text input to allow pasting or typing product names
    function renderProductsTab(container, trialId) {
      const arms = getArms(trialId);
      // Products linked to trial with arm info
      const trialProds = trial_products.filter(tp => tp.trial_id === trialId);

      let html = `
        <div class="mb-4 flex flex-col md:flex-row md:items-center md:justify-between gap-4">
          <h3 class="text-xl font-semibold text-blue-900">Products (ARM-wise)</h3>
          <button id="showAddProductFormBtn" class="bg-green-700 text-white px-4 py-2 rounded hover:bg-green-600 transition text-sm flex items-center gap-2">
            <i class="fas fa-plus"></i> Add Product
          </button>
        </div>
      `;

      if (trialProds.length === 0) {
        html += `<p class="text-gray-600 italic mb-4">No products added yet.</p>`;
      } else {
        html += `<div class="overflow-x-auto max-h-64 scrollbar-thin border border-gray-300 rounded">
          <table class="min-w-full border-collapse border border-gray-300 text-sm">
            <thead class="bg-blue-900 text-white">
              <tr>
                <th class="px-3 py-2 text-left">ARM</th>
                <th class="px-3 py-2 text-left">Product Name</th>
                <th class="px-3 py-2 text-left">Dose</th>
                <th class="px-3 py-2 text-left">Dosage Details</th>
                <th class="px-3 py-2 text-left">Actions</th>
              </tr>
            </thead>
            <tbody>
              ${trialProds.map(tp => {
                return `<tr class="border-t border-gray-200 hover:bg-gray-100">
                  <td class="px-3 py-1">${tp.arm}</td>
                  <td class="px-3 py-1">${tp.product_name || ''}</td>
                  <td class="px-3 py-1">${tp.dose || ''}</td>
                  <td class="px-3 py-1">${tp.dosage_details || ''}</td>
                  <td class="px-3 py-1">
                    <button data-tp-id="${tp.id}" class="edit-product-btn text-blue-700 hover:underline text-sm">Edit</button>
                    <button data-tp-id="${tp.id}" class="remove-product-btn text-red-600 hover:underline text-sm ml-2">Remove</button>
                  </td>
                </tr>`;
              }).join('')}
            </tbody>
          </table>
        </div>`;
      }

      // Add Product Form (hidden initially)
      html += `
        <form id="addProductForm" class="mt-6 bg-gray-50 p-4 rounded shadow-md max-w-4xl hidden grid grid-cols-1 md:grid-cols-2 gap-4" novalidate>
          <h4 class="md:col-span-2 text-lg font-semibold text-blue-900">Add / Edit Product (ARM-wise)</h4>
          <input type="hidden" id="productEditId" name="product_edit_id" value="" />
          <div>
            <label for="productArm" class="block font-medium mb-1">ARM *</label>
            <input type="text" id="productArm" name="arm" placeholder="e.g. ARM 1" class="w-full border border-gray-300 rounded px-3 py-2 focus:outline-none focus:ring-2 focus:ring-blue-600" list="armsList" required />
            <datalist id="armsList">${arms.map(a => `<option value="${a}"></option>`).join('')}</datalist>
          </div>
          <div>
            <label for="productName" class="block font-medium mb-1">Product Name *</label>
            <input type="text" id="productName" name="product_name" placeholder="Product name (free text)" class="w-full border border-gray-300 rounded px-3 py-2 focus:outline-none focus:ring-2 focus:ring-blue-600" required />
          </div>
          <div>
            <label for="productDose" class="block font-medium mb-1">Dose</label>
            <input type="text" id="productDose" name="dose" placeholder="Dose" class="w-full border border-gray-300 rounded px-3 py-2 focus:outline-none focus:ring-2 focus:ring-blue-600" />
          </div>
          <div>
            <label for="productDosageDetails" class="block font-medium mb-1">Dosage Details</label>
            <textarea id="productDosageDetails" name="dosage_details" rows="3" placeholder="Dosage details" class="w-full border border-gray-300 rounded px-3 py-2 focus:outline-none focus:ring-2 focus:ring-blue-600 resize-y"></textarea>
          </div>
          <div class="md:col-span-2">
            <label for="productSourceName" class="block font-medium mb-1">Reference Source Name</label>
            <input type="text" id="productSourceName" name="source_name" placeholder="Source name" class="w-full border border-gray-300 rounded px-3 py-2 focus:outline-none focus:ring-2 focus:ring-blue-600" />
          </div>
          <div class="md:col-span-2">
            <label for="productReferenceLink" class="block font-medium mb-1">Reference Link</label>
            <input type="url" id="productReferenceLink" name="reference_link" placeholder="https://example.com" class="w-full border border-gray-300 rounded px-3 py-2 focus:outline-none focus:ring-2 focus:ring-blue-600" />
          </div>
          <div class="md:col-span-2 flex justify-end gap-4">
            <button type="button" id="cancelProductBtn" class="bg-gray-400 text-white font-semibold rounded px-6 py-2 hover:bg-gray-500 transition">Cancel</button>
            <button type="submit" class="bg-green-700 text-white font-semibold rounded px-6 py-2 hover:bg-green-600 transition">
              <i class="fas fa-save mr-2"></i> Save Product
            </button>
          </div>
          <div id="productFormMessage" class="md:col-span-2 text-sm mt-2"></div>
        </form>
      `;

      container.innerHTML = html;

      // Event handlers
      document.getElementById('showAddProductFormBtn').addEventListener('click', () => {
        resetProductForm();
        document.getElementById('addProductForm').classList.remove('hidden');
        document.getElementById('productArm').focus();
      });

      document.getElementById('cancelProductBtn').addEventListener('click', () => {
        resetProductForm();
        document.getElementById('addProductForm').classList.add('hidden');
      });

      document.getElementById('addProductForm').addEventListener('submit', e => {
        e.preventDefault();
        const form = e.target;
        const editId = form.product_edit_id.value;
        const arm = form.arm.value.trim();
        const product_name = form.product_name.value.trim();
        if (!arm || !product_name) {
          showProductFormMessage('ARM and Product Name are required.', true);
          return;
        }
        const dose = form.dose.value.trim() || null;
        const dosage_details = form.dosage_details.value.trim() || null;
        const source_name = form.source_name.value.trim() || null;
        const reference_link = form.reference_link.value.trim() || null;

        // Add arm if new
        addArm(currentTrialId, arm);

        if (editId) {
          // Edit existing trial_product entry
          const tpId = parseInt(editId);
          const tpIndex = trial_products.findIndex(tp => tp.id === tpId);
          if (tpIndex === -1) {
            showProductFormMessage('Product entry not found.', true);
            return;
          }
          trial_products[tpIndex].arm = arm;
          trial_products[tpIndex].product_name = product_name;
          trial_products[tpIndex].dose = dose;
          trial_products[tpIndex].dosage_details = dosage_details;
          showProductFormMessage('Product updated successfully.');
        } else {
          // Add new trial_product entry
          trial_products.push({
            id: generateId(trial_products),
            trial_id: currentTrialId,
            arm,
            product_name,
            dose,
            dosage_details
          });
          showProductFormMessage('Product added successfully.');
        }

        // Add reference if provided
        if (source_name && reference_link) {
          addReference(currentTrialId, 'products', source_name, reference_link);
        }

        loadTabContent('products');
      });

      container.querySelectorAll('.edit-product-btn').forEach(btn => {
        btn.addEventListener('click', () => {
          const tpId = parseInt(btn.getAttribute('data-tp-id'));
          const tp = trial_products.find(t => t.id === tpId);
          if (!tp) return;
          const form = document.getElementById('addProductForm');
          form.product_edit_id.value = tp.id;
          form.arm.value = tp.arm;
          form.product_name.value = tp.product_name || '';
          form.dose.value = tp.dose || '';
          form.dosage_details.value = tp.dosage_details || '';
          form.source_name.value = '';
          form.reference_link.value = '';
          document.getElementById('addProductForm').classList.remove('hidden');
          form.arm.focus();
        });
      });

      container.querySelectorAll('.remove-product-btn').forEach(btn => {
        btn.addEventListener('click', () => {
          const tpId = parseInt(btn.getAttribute('data-tp-id'));
          const idx = trial_products.findIndex(tp => tp.id === tpId);
          if (idx !== -1) trial_products.splice(idx, 1);
          loadTabContent('products');
        });
      });

      function resetProductForm() {
        const form = document.getElementById('addProductForm');
        form.reset();
        form.product_edit_id.value = '';
        showProductFormMessage('');
      }
      function showProductFormMessage(msg, isError = false) {
        const el = document.getElementById('productFormMessage');
        el.textContent = msg;
        el.className = isError ? 'text-sm mt-2 text-red-600' : 'text-sm mt-2 text-green-600';
        if (msg) setTimeout(() => { el.textContent = ''; }, 4000);
      }
    }

    // Initialize dynamic inputs on page load
    window.addEventListener('load', () => {
      // Initialize add trial form dynamic inputs with one input each
      const addOtherStudyIdsContainer = document.getElementById('addOtherStudyIdsContainer');
      addOtherStudyIdsContainer.innerHTML = '';
      const firstOtherStudyInput = document.createElement('input');
      firstOtherStudyInput.type = 'text';
      firstOtherStudyInput.name = 'other_study_id';
      firstOtherStudyInput.placeholder = 'Other Study ID';
      firstOtherStudyInput.className = 'w-full border border-gray-300 rounded px-3 py-2 focus:outline-none focus:ring-2 focus:ring-blue-600';
      addOtherStudyIdsContainer.appendChild(firstOtherStudyInput);

      const addIndicationsContainer = document.getElementById('addIndicationsContainer');
      addIndicationsContainer.innerHTML = '';
      const firstIndicationInput = document.createElement('input');
      firstIndicationInput.type = 'text';
      firstIndicationInput.name = 'indication';
      firstIndicationInput.placeholder = 'Indication';
      firstIndicationInput.className = 'w-full border border-gray-300 rounded px-3 py-2 focus:outline-none focus:ring-2 focus:ring-blue-600';
      addIndicationsContainer.appendChild(firstIndicationInput);

      const productTagsContainer = document.getElementById('productTagsContainer');
      productTagsContainer.innerHTML = '';
      const firstProductTagInput = document.createElement('input');
      firstProductTagInput.type = 'text';
      firstProductTagInput.name = 'product_tag';
      firstProductTagInput.placeholder = 'Product name';
      firstProductTagInput.className = 'w-full border border-gray-300 rounded px-3 py-2 focus:outline-none focus:ring-2 focus:ring-blue-600';
      productTagsContainer.appendChild(firstProductTagInput);

      // Initialize search form dynamic inputs with one input each
      const searchOtherStudyIdsContainer = document.getElementById('searchOtherStudyIdsContainer');
      searchOtherStudyIdsContainer.innerHTML = '';
      const firstSearchOtherStudyInput = document.createElement('input');
      firstSearchOtherStudyInput.type = 'text';
      firstSearchOtherStudyInput.name = 'other_study_id';
      firstSearchOtherStudyInput.placeholder = 'Other Study ID';
      firstSearchOtherStudyInput.className = 'w-full border border-gray-300 rounded px-3 py-2 focus:outline-none focus:ring-2 focus:ring-blue-600';
      searchOtherStudyIdsContainer.appendChild(firstSearchOtherStudyInput);

      const searchIndicationsContainer = document.getElementById('searchIndicationsContainer');
      searchIndicationsContainer.innerHTML = '';
      const firstSearchIndicationInput = document.createElement('input');
      firstSearchIndicationInput.type = 'text';
      firstSearchIndicationInput.name = 'indication';
      firstSearchIndicationInput.placeholder = 'Indication';
      firstSearchIndicationInput.className = 'w-full border border-gray-300 rounded px-3 py-2 focus:outline-none focus:ring-2 focus:ring-blue-600';
      searchIndicationsContainer.appendChild(firstSearchIndicationInput);
    });
  </script>
</body>
</html>
