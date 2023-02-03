<template>
  <div class="container-fluid">
    <div class="row">
      <nav
        id="sidebarMenu"
        class="col-md-3 col-lg-2 d-md-block bg-light sidebar collapse"
      >
        <div class="position-sticky pt-3 sidebar-sticky">
          <h5>Menu</h5>
          <ul class="nav flex-column">
            <li class="nav-item">
              <a class="nav-link active" aria-current="page" href="#">
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  width="24"
                  height="24"
                  viewBox="0 0 24 24"
                  fill="none"
                  stroke="currentColor"
                  stroke-width="2"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  class="feather feather-home align-text-bottom"
                  aria-hidden="true"
                >
                  <path
                    d="M3 9l9-7 9 7v11a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2z"
                  ></path>
                  <polyline points="9 22 9 12 15 12 15 22"></polyline>
                </svg>
                Dashboard
              </a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  width="24"
                  height="24"
                  viewBox="0 0 24 24"
                  fill="none"
                  stroke="currentColor"
                  stroke-width="2"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  class="feather feather-file align-text-bottom"
                  aria-hidden="true"
                >
                  <path
                    d="M13 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V9z"
                  ></path>
                  <polyline points="13 2 13 9 20 9"></polyline>
                </svg>
                Orders
              </a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  width="24"
                  height="24"
                  viewBox="0 0 24 24"
                  fill="none"
                  stroke="currentColor"
                  stroke-width="2"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  class="feather feather-shopping-cart align-text-bottom"
                  aria-hidden="true"
                >
                  <circle cx="9" cy="21" r="1"></circle>
                  <circle cx="20" cy="21" r="1"></circle>
                  <path
                    d="M1 1h4l2.68 13.39a2 2 0 0 0 2 1.61h9.72a2 2 0 0 0 2-1.61L23 6H6"
                  ></path>
                </svg>
                Products
              </a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  width="24"
                  height="24"
                  viewBox="0 0 24 24"
                  fill="none"
                  stroke="currentColor"
                  stroke-width="2"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  class="feather feather-users align-text-bottom"
                  aria-hidden="true"
                >
                  <path d="M17 21v-2a4 4 0 0 0-4-4H5a4 4 0 0 0-4 4v2"></path>
                  <circle cx="9" cy="7" r="4"></circle>
                  <path d="M23 21v-2a4 4 0 0 0-3-3.87"></path>
                  <path d="M16 3.13a4 4 0 0 1 0 7.75"></path>
                </svg>
                Customers
              </a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  width="24"
                  height="24"
                  viewBox="0 0 24 24"
                  fill="none"
                  stroke="currentColor"
                  stroke-width="2"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  class="feather feather-bar-chart-2 align-text-bottom"
                  aria-hidden="true"
                >
                  <line x1="18" y1="20" x2="18" y2="10"></line>
                  <line x1="12" y1="20" x2="12" y2="4"></line>
                  <line x1="6" y1="20" x2="6" y2="14"></line>
                </svg>
                Reports
              </a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  width="24"
                  height="24"
                  viewBox="0 0 24 24"
                  fill="none"
                  stroke="currentColor"
                  stroke-width="2"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  class="feather feather-layers align-text-bottom"
                  aria-hidden="true"
                >
                  <polygon points="12 2 2 7 12 12 22 7 12 2"></polygon>
                  <polyline points="2 17 12 22 22 17"></polyline>
                  <polyline points="2 12 12 17 22 12"></polyline>
                </svg>
                Integrations
              </a>
            </li>
          </ul>

          <h6
            class="sidebar-heading d-flex justify-content-between align-items-center px-3 mt-4 mb-1 text-muted text-uppercase"
          >
            <span>Saved reports</span>
            <a class="link-secondary" href="#" aria-label="Add a new report">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                width="24"
                height="24"
                viewBox="0 0 24 24"
                fill="none"
                stroke="currentColor"
                stroke-width="2"
                stroke-linecap="round"
                stroke-linejoin="round"
                class="feather feather-plus-circle align-text-bottom"
                aria-hidden="true"
              >
                <circle cx="12" cy="12" r="10"></circle>
                <line x1="12" y1="8" x2="12" y2="16"></line>
                <line x1="8" y1="12" x2="16" y2="12"></line>
              </svg>
            </a>
          </h6>
          <ul class="nav flex-column mb-2">
            <li class="nav-item">
              <a class="nav-link" href="#">
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  width="24"
                  height="24"
                  viewBox="0 0 24 24"
                  fill="none"
                  stroke="currentColor"
                  stroke-width="2"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  class="feather feather-file-text align-text-bottom"
                  aria-hidden="true"
                >
                  <path
                    d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"
                  ></path>
                  <polyline points="14 2 14 8 20 8"></polyline>
                  <line x1="16" y1="13" x2="8" y2="13"></line>
                  <line x1="16" y1="17" x2="8" y2="17"></line>
                  <polyline points="10 9 9 9 8 9"></polyline>
                </svg>
                Current month
              </a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  width="24"
                  height="24"
                  viewBox="0 0 24 24"
                  fill="none"
                  stroke="currentColor"
                  stroke-width="2"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  class="feather feather-file-text align-text-bottom"
                  aria-hidden="true"
                >
                  <path
                    d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"
                  ></path>
                  <polyline points="14 2 14 8 20 8"></polyline>
                  <line x1="16" y1="13" x2="8" y2="13"></line>
                  <line x1="16" y1="17" x2="8" y2="17"></line>
                  <polyline points="10 9 9 9 8 9"></polyline>
                </svg>
                Last quarter
              </a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  width="24"
                  height="24"
                  viewBox="0 0 24 24"
                  fill="none"
                  stroke="currentColor"
                  stroke-width="2"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  class="feather feather-file-text align-text-bottom"
                  aria-hidden="true"
                >
                  <path
                    d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"
                  ></path>
                  <polyline points="14 2 14 8 20 8"></polyline>
                  <line x1="16" y1="13" x2="8" y2="13"></line>
                  <line x1="16" y1="17" x2="8" y2="17"></line>
                  <polyline points="10 9 9 9 8 9"></polyline>
                </svg>
                Social engagement
              </a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  width="24"
                  height="24"
                  viewBox="0 0 24 24"
                  fill="none"
                  stroke="currentColor"
                  stroke-width="2"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  class="feather feather-file-text align-text-bottom"
                  aria-hidden="true"
                >
                  <path
                    d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"
                  ></path>
                  <polyline points="14 2 14 8 20 8"></polyline>
                  <line x1="16" y1="13" x2="8" y2="13"></line>
                  <line x1="16" y1="17" x2="8" y2="17"></line>
                  <polyline points="10 9 9 9 8 9"></polyline>
                </svg>
                Year-end sale
              </a>
            </li>
          </ul>
        </div>
      </nav>

      <main class="col-md-9 ms-sm-auto col-lg-10 px-md-4">
        <div class="chartjs-size-monitor">
          <div class="chartjs-size-monitor-expand"><div class=""></div></div>
          <div class="chartjs-size-monitor-shrink"><div class=""></div></div>
        </div>
        <div
          class="d-flex justify-content-between flex-wrap flex-md-nowrap align-items-center pt-3 pb-2 mb-3 border-bottom"
        >
          <h1 class="h2">Dashboard</h1>
          <div class="btn-toolbar mb-2 mb-md-0">
            <div class="btn-group me-2">
              <button type="button" class="btn btn-sm btn-outline-secondary">
                Share
              </button>
              <button type="button" class="btn btn-sm btn-outline-secondary">
                Export
              </button>
            </div>
            <button
              type="button"
              class="btn btn-sm btn-outline-secondary dropdown-toggle"
            >
              <svg
                xmlns="http://www.w3.org/2000/svg"
                width="24"
                height="24"
                viewBox="0 0 24 24"
                fill="none"
                stroke="currentColor"
                stroke-width="2"
                stroke-linecap="round"
                stroke-linejoin="round"
                class="feather feather-calendar align-text-bottom"
                aria-hidden="true"
              >
                <rect x="3" y="4" width="18" height="18" rx="2" ry="2"></rect>
                <line x1="16" y1="2" x2="16" y2="6"></line>
                <line x1="8" y1="2" x2="8" y2="6"></line>
                <line x1="3" y1="10" x2="21" y2="10"></line>
              </svg>
              This week
            </button>
          </div>
        </div>

        <img
          src="data:image/png;base64,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"
          class="w-25 mx-5"
          alt=""
        />
        <img
          src="data:image/png;base64,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"
          alt=""
          class="w-25 mx-5"
        />
        <img
          src="https://media.istockphoto.com/id/1157569047/photo/red-arrow-moving-up-over-graph-paper-background.jpg?s=612x612&w=0&k=20&c=h_mHs726U_Osy2IapdLYJCfZHQoh8oxfG_lJoG4SwXI="
          alt=""
          class="w-25 mx-5"
        />
        <h2>Section title</h2>
        <div class="table-responsive">
          <table class="table table-striped table-sm">
            <thead>
              <tr>
                <th scope="col">#</th>
                <th scope="col">Header</th>
                <th scope="col">Header</th>
                <th scope="col">Header</th>
                <th scope="col">Header</th>
              </tr>
            </thead>
            <tbody>
              <tr>
                <td>1,001</td>
                <td>random</td>
                <td>data</td>
                <td>placeholder</td>
                <td>text</td>
              </tr>
              <tr>
                <td>1,002</td>
                <td>placeholder</td>
                <td>irrelevant</td>
                <td>visual</td>
                <td>layout</td>
              </tr>
              <tr>
                <td>1,003</td>
                <td>data</td>
                <td>rich</td>
                <td>dashboard</td>
                <td>tabular</td>
              </tr>
              <tr>
                <td>1,003</td>
                <td>information</td>
                <td>placeholder</td>
                <td>illustrative</td>
                <td>data</td>
              </tr>
              <tr>
                <td>1,004</td>
                <td>text</td>
                <td>random</td>
                <td>layout</td>
                <td>dashboard</td>
              </tr>
              <tr>
                <td>1,005</td>
                <td>dashboard</td>
                <td>irrelevant</td>
                <td>text</td>
                <td>placeholder</td>
              </tr>
              <tr>
                <td>1,006</td>
                <td>dashboard</td>
                <td>illustrative</td>
                <td>rich</td>
                <td>data</td>
              </tr>
              <tr>
                <td>1,007</td>
                <td>placeholder</td>
                <td>tabular</td>
                <td>information</td>
                <td>irrelevant</td>
              </tr>
              <tr>
                <td>1,008</td>
                <td>random</td>
                <td>data</td>
                <td>placeholder</td>
                <td>text</td>
              </tr>
              <tr>
                <td>1,009</td>
                <td>placeholder</td>
                <td>irrelevant</td>
                <td>visual</td>
                <td>layout</td>
              </tr>
              <tr>
                <td>1,010</td>
                <td>data</td>
                <td>rich</td>
                <td>dashboard</td>
                <td>tabular</td>
              </tr>
              <tr>
                <td>1,011</td>
                <td>information</td>
                <td>placeholder</td>
                <td>illustrative</td>
                <td>data</td>
              </tr>
              <tr>
                <td>1,012</td>
                <td>text</td>
                <td>placeholder</td>
                <td>layout</td>
                <td>dashboard</td>
              </tr>
              <tr>
                <td>1,013</td>
                <td>dashboard</td>
                <td>irrelevant</td>
                <td>text</td>
                <td>visual</td>
              </tr>
              <tr>
                <td>1,014</td>
                <td>dashboard</td>
                <td>illustrative</td>
                <td>rich</td>
                <td>data</td>
              </tr>
              <tr>
                <td>1,015</td>
                <td>random</td>
                <td>tabular</td>
                <td>information</td>
                <td>text</td>
              </tr>
            </tbody>
          </table>
        </div>
      </main>
    </div>
  </div>
</template>

<style>
.td {
  text-decoration: none;
}
</style>
