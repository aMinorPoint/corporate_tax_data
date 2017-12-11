# Data on corporate taxes and how companies use their profits
The data below was used to create [this](http://www.aminorpoint.com/blog/corporate_taxes_and_profit_uses/) post exploring corporate income taxes in the US.

# Data files and sources sources
<ul>
<li>federal_corporate_tax_receipts.csv - Tax recepits be year, in $ billions - available in the <a href="https://www.fiscal.treasury.gov/fsreports/rpt/mthTreasStmt/backissues.htm"><u>Monthly Treasury Statements</u></a> from the US Department of the Treasury.</li>
			<br>
			<li>2013_corporate_tax_by_size.csv - Corporate taxes broken down by company size - available in the IRS' <a href="https://www.irs.gov/statistics/soi-tax-stats-corporation-complete-report"><u>Corporation Complete Report</u></a> under Table 5.  Lots of other interesting data available here, including breakdowns by industry.</li>
			<br>
			<li>BEA_corp_profits_after_tax_simple.csv - Corporate profits, in $ billions - available from the St. Louis Fed's <a href="https://fred.stlouisfed.org/series/CPATAX"><u>FRED</u></a> system.  The original reports are put out by the Bureau of Economic Analysis as part of the GDP report.  The data can be found <a href="https://www.bea.gov/iTable/iTable.cfm?reqid=19&step=2#reqid=19&step=2&isuri=1&1921=survey"><u>here</u></a> under Table 6.19.  Note that the corporate tax information contained in these tables does not match the information from the Treasury Department.  This is due to different classifications of payments from the Federal Reserve to the government.  From the BEA, those payments are included under corporate income taxes.  But they are classified separately by the Treasury Department.  See <a href="https://www.bea.gov/faq/index.cfm?faq_id=510"><u>this</u></a> for more clarification. I used the data excluding the Federal Reserve payments since they are due to the Fed's Quantitative Easing program, and are not affected by corporate tax policy.</li>
			<br>
			<li>fixed_capital_formation.csv - Corporate fixed investment, in $ billions - available in <a href="https://fred.stlouisfed.org/series/NCBGCFQ027S"><u>FRED</u></a> and originally from the Federal Reserve's <a href="https://www.federalreserve.gov/releases/z1/"><u>Financial Accounts of the United States</u></a>.</li>
			<br>
			<li>shareholder_returns.csv - Dividends and Share Repurchases, in $ billions - The dividend data is available in <a href="https://fred.stlouisfed.org/series/B056RC1A027NBEA"><u>FRED</u></a> and originally from the BEA's GDP reports and <a href="https://www.bea.gov/iTable/iTable.cfm?reqid=19&step=2#reqid=19&step=2&isuri=1&1921=survey"><u>NIPA tables</u></a>.  Share repurchase data is available from the Federal Reserve's <a href="https://www.federalreserve.gov/releases/efa/efa-project-equity-issuance-retirement.htm"><u>Enhanced Financial Accounts</u></a>.  Note that this is only for "nonfinancial corporations" which excludes the financial sector.  So it underestimates total share repurchases for all corporations as the big banks are currently executing share repurchase programs.</li>
