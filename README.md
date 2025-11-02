<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Career Site Analytics - Glossary</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Arial, sans-serif;
            background-color: #f5f5f5;
            color: #333;
            line-height: 1.6;
        }
        
        .header {
            background-color: #00bcd4;
            color: white;
            padding: 24px;
            margin-bottom: 24px;
        }
        
        .header h1 {
            font-size: 24px;
            font-weight: 500;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 24px 48px;
        }
        
        .search-box {
            background: white;
            padding: 20px;
            border-radius: 4px;
            margin-bottom: 24px;
            box-shadow: 0 1px 3px rgba(0,0,0,0.1);
        }
        
        .search-box input {
            width: 100%;
            padding: 12px;
            border: 1px solid #ddd;
            border-radius: 4px;
            font-size: 14px;
        }
        
        .search-box input:focus {
            outline: none;
            border-color: #00bcd4;
        }
        
        .section {
            background: white;
            padding: 24px;
            margin-bottom: 24px;
            border-radius: 4px;
            box-shadow: 0 1px 3px rgba(0,0,0,0.1);
        }
        
        .section-header {
            background-color: #00bcd4;
            color: white;
            padding: 12px 16px;
            margin: -24px -24px 20px -24px;
            border-radius: 4px 4px 0 0;
            font-size: 16px;
            font-weight: 500;
        }
        
        .term-item {
            padding: 16px 0;
            border-bottom: 1px solid #f0f0f0;
        }
        
        .term-item:last-child {
            border-bottom: none;
        }
        
        .term-name {
            font-weight: 600;
            color: #00bcd4;
            font-size: 15px;
            margin-bottom: 8px;
        }
        
        .term-definition {
            color: #555;
            font-size: 14px;
            line-height: 1.6;
        }
        
        .formula {
            background-color: #f9f9f9;
            padding: 8px 12px;
            border-left: 3px solid #00bcd4;
            margin-top: 8px;
            font-family: 'Courier New', monospace;
            font-size: 13px;
            color: #666;
        }
        
        .note {
            background-color: #e3f2fd;
            padding: 12px;
            margin-top: 8px;
            border-radius: 4px;
            font-size: 13px;
            color: #1976d2;
        }
        
        .no-results {
            text-align: center;
            padding: 40px;
            color: #999;
            display: none;
        }
    </style>
</head>
<body>
    <div class="header">
        <h1>Career Site Analytics - Glossary & Definitions</h1>
    </div>
    
    <div class="container">
        <div class="search-box">
            <input type="text" id="searchInput" placeholder="Search for a term or metric...">
        </div>
        
        <div class="no-results" id="noResults">No terms found matching your search.</div>
        
        <div class="section" data-section="traffic">
            <div class="section-header">Traffic & Reach Metrics</div>
            
            <div class="term-item">
                <div class="term-name">Total Candidate Visits</div>
                <div class="term-definition">
                    The total number of sessions (visits) to your career site during the selected time period. A single user may account for multiple visits if they return to the site at different times.
                </div>
                <div class="formula">Source: GA4 Sessions metric</div>
            </div>
            
            <div class="term-item">
                <div class="term-name">Unique Candidates</div>
                <div class="term-definition">
                    The number of distinct visitors to your career site, identified by unique browser cookies or user IDs. This represents individual people rather than repeat visits.
                </div>
                <div class="formula">Source: GA4 Total Users metric</div>
            </div>
            
            <div class="term-item">
                <div class="term-name">Total Users</div>
                <div class="term-definition">
                    All users who visited the career site within the specified date range. This is measured using GA4's user identification methods (cookies, User ID, etc.).
                </div>
            </div>
            
            <div class="term-item">
                <div class="term-name">Total Apply Clicks</div>
                <div class="term-definition">
                    The cumulative number of times candidates clicked on an "Apply" button across your career site. This includes multiple clicks from the same user and applies to all job postings.
                </div>
                <div class="note">Note: A high number of apply clicks relative to applications may indicate issues with the application process.</div>
            </div>
        </div>
        
        <div class="section" data-section="engagement">
            <div class="section-header">Engagement Metrics</div>
            
            <div class="term-item">
                <div class="term-name">Avg Eng Time per User</div>
                <div class="term-definition">
                    Average Engagement Time per User - The mean amount of time users spent actively engaged with your career site content. This only counts time when the browser tab is in focus and the user is interacting with the page.
                </div>
                <div class="formula">Formula: Total Engagement Time ÷ Total Users</div>
            </div>
            
            <div class="term-item">
                <div class="term-name">Talent Network Opt-ins</div>
                <div class="term-definition">
                    The total number of times candidates subscribed to your talent network, job alerts, or newsletter. This may include duplicate opt-ins from the same individual.
                </div>
            </div>
            
            <div class="term-item">
                <div class="term-name">Unique Talent Network Opt-ins</div>
                <div class="term-definition">
                    The number of distinct candidates who joined your talent network, counting each person only once regardless of how many times they may have attempted to opt in.
                </div>
            </div>
            
            <div class="term-item">
                <div class="term-name">Talent Network Opt-in Rate</div>
                <div class="term-definition">
                    The percentage of career site visitors who opted into your talent network or job alerts program during their visit.
                </div>
                <div class="formula">Formula: (Unique Opt-ins ÷ Unique Candidates) × 100</div>
            </div>
        </div>
        
        <div class="section" data-section="conversion">
            <div class="section-header">Conversion Metrics</div>
            
            <div class="term-item">
                <div class="term-name">Apply Clicks (Selected)</div>
                <div class="term-definition">
                    The number of apply button clicks for the currently filtered segment (e.g., specific job category, location, or source). This helps you understand conversion performance for specific audience segments.
                </div>
            </div>
            
            <div class="term-item">
                <div class="term-name">Apply Rate (Selected)</div>
                <div class="term-definition">
                    The percentage of visitors in the selected filter group who clicked an apply button. This conversion rate helps identify which segments are most engaged with your opportunities.
                </div>
                <div class="formula">Formula: (Apply Clicks ÷ Total Users in segment) × 100</div>
            </div>
            
            <div class="term-item">
                <div class="term-name">Views</div>
                <div class="term-definition">
                    Total page views or job listing views for the selected dimension. This represents how many times content was displayed to users.
                </div>
            </div>
            
            <div class="term-item">
                <div class="term-name">Apply Click Value</div>
                <div class="term-definition">
                    A metric showing the quality or value of apply clicks, which may incorporate factors like completion rate, time to hire, or applicant quality scores.
                </div>
            </div>
        </div>
        
        <div class="section" data-section="dimensions">
            <div class="section-header">Dimensions & Filters</div>
            
            <div class="term-item">
                <div class="term-name">Career Site Dimension</div>
                <div class="term-definition">
                    The method by which data is segmented and analyzed. Common dimensions include traffic source, job category, location, device type, and campaign attribution.
                </div>
            </div>
            
            <div class="term-item">
                <div class="term-name">Grouped Source</div>
                <div class="term-definition">
                    A categorization of where your traffic originates, typically grouped into categories like organic search, direct, marketing/paid, social, referral, and email campaigns.
                </div>
            </div>
            
            <div class="term-item">
                <div class="term-name">Job Category</div>
                <div class="term-definition">
                    The functional area or department classification of job postings (e.g., Engineering, Marketing, Sales, Operations, Finance).
                </div>
            </div>
            
            <div class="term-item">
                <div class="term-name">Job Title</div>
                <div class="term-definition">
                    The specific role name or position title as it appears in job listings.
                </div>
            </div>
            
            <div class="term-item">
                <div class="term-name">Job Location</div>
                <div class="term-definition">
                    The geographic location where a position is based, which may include city, state/province, country, or "Remote" designations.
                </div>
            </div>
            
            <div class="term-item">
                <div class="term-name">Req ID / Type In</div>
                <div class="term-definition">
                    The unique requisition identifier assigned to each job opening in your applicant tracking system (ATS). Used for tracking specific job performance.
                </div>
            </div>
            
            <div class="term-item">
                <div class="term-name">City / State</div>
                <div class="term-definition">
                    Geographic filters that allow you to analyze candidate behavior and engagement by their location or by job location.
                </div>
            </div>
        </div>
        
        <div class="section" data-section="sources">
            <div class="section-header">Traffic Sources</div>
            
            <div class="term-item">
                <div class="term-name">Direct</div>
                <div class="term-definition">
                    Traffic from users who typed your career site URL directly into their browser, used a bookmark, or came from an untrackable source (e.g., non-web documents, untagged emails).
                </div>
            </div>
            
            <div class="term-item">
                <div class="term-name">Organic Search</div>
                <div class="term-definition">
                    Visitors who found your career site through unpaid search engine results (Google, Bing, etc.). This indicates strong SEO performance and employer brand awareness.
                </div>
            </div>
            
            <div class="term-item">
                <div class="term-name">Marketing</div>
                <div class="term-definition">
                    Traffic generated from paid marketing campaigns, including pay-per-click ads, display advertising, sponsored job postings, and other paid promotional activities.
                </div>
            </div>
            
            <div class="term-item">
                <div class="term-name">LinkedIn</div>
                <div class="term-definition">
                    Traffic originating from LinkedIn, including both organic posts and paid LinkedIn advertising campaigns.
                </div>
            </div>
            
            <div class="term-item">
                <div class="term-name">Indeed</div>
                <div class="term-definition">
                    Candidates who clicked through from job listings on Indeed.com, one of the largest job aggregation platforms.
                </div>
            </div>
            
            <div class="term-item">
                <div class="term-name">Google</div>
                <div class="term-definition">
                    Traffic from Google sources, including organic search, Google for Jobs, and Google Ads campaigns.
                </div>
            </div>
            
            <div class="term-item">
                <div class="term-name">Talent Network / Ecosystem</div>
                <div class="term-definition">
                    Candidates who arrived via your talent community, previous applicant database, or recruitment marketing automation platforms.
                </div>
            </div>
        </div>
        
        <div class="section" data-section="technical">
            <div class="section-header">Technical Terms</div>
            
            <div class="term-item">
                <div class="term-name">GA4</div>
                <div class="term-definition">
                    Google Analytics 4 - The latest version of Google's web analytics platform, which uses event-based tracking rather than session-based tracking. This is the data source for your career site dashboard.
                </div>
            </div>
            
            <div class="term-item">
                <div class="term-name">Looker</div>
                <div class="term-definition">
                    The business intelligence and data visualization platform used to create this dashboard. Looker connects to GA4 data to provide real-time career site analytics.
                </div>
            </div>
            
            <div class="term-item">
                <div class="term-name">Date Range</div>
                <div class="term-definition">
                    The time period selected for analysis. Adjusting the date range allows you to compare performance across different weeks, months, or quarters.
                </div>
            </div>
            
            <div class="term-item">
                <div class="term-name">Selected Career Site Dimension</div>
                <div class="term-definition">
                    The currently active filter or grouping applied to the data, which determines how metrics are segmented and displayed in the dashboard.
                </div>
            </div>
        </div>
    </div>
    
    <script>
        const searchInput = document.getElementById('searchInput');
        const sections = document.querySelectorAll('.section');
        const noResults = document.getElementById('noResults');
        
        searchInput.addEventListener('input', function(e) {
            const searchTerm = e.target.value.toLowerCase();
            let hasResults = false;
            
            sections.forEach(section => {
                const terms = section.querySelectorAll('.term-item');
                let sectionHasVisibleTerms = false;
                
                terms.forEach(term => {
                    const termName = term.querySelector('.term-name').textContent.toLowerCase();
                    const termDef = term.querySelector('.term-definition').textContent.toLowerCase();
                    
                    if (termName.includes(searchTerm) || termDef.includes(searchTerm) || searchTerm === '') {
                        term.style.display = 'block';
                        sectionHasVisibleTerms = true;
                        hasResults = true;
                    } else {
                        term.style.display = 'none';
                    }
                });
                
                section.style.display = sectionHasVisibleTerms ? 'block' : 'none';
            });
            
            noResults.style.display = hasResults ? 'none' : 'block';
        });
    </script>
</body>
</html>
