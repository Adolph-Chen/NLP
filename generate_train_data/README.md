# 全部意图

```

    // 报表类意图
    EXPENSE_ANALYSIS_QUERY("expense_analysis", "费用分析", "ai_report", "", "expense_analysis"),

    FINANCIAL_ANALYSIS_REPORT_QUERY("financial_analysis_report", "财务分析报告", "ai_report", "", "financial_analysis_report"),

    FUND_ANALYSIS_QUERY("fund_analysis", "资金分析", "ai_report", "", "fund_analysis"),

    LAST_MONTH_MANAGEMENT_ACCOUNTING_PROFIT_LOSS_STATEMENT_PRINT("last_month_management_accounting_profit_loss_statement_analysis", "上月管理会计损益表", "ai_report", "", "management_accounting_profit_loss_statement_print"),

    LAST_MONTH_PROFIT_LOSS_BALANCE_ANALYSIS_REPORT_PRINT("last_month_profit_loss_balance_analysis_report_analysis", "上个月盈亏平衡分析报告", "ai_report", "", "management_accounting_profit_loss_statement_print"),

    OBSOLETE_INVENTORY_ANALYSIS_PRINT("obsolete_inventory_analysis", "呆滞库存分析", "ai_report", "", "obsolete_inventory_analysis_print"),

    PURCHASE_COST_ANALYSIS_QUERY("purchase_cost_analysis", "采购成本分析", "ai_report", "", "purchase_cost_analysis"),

    TOP_X_CUSTOMER_PROFIT_ANALYSIS_PRINT("top_x_customer_profit_analysis_analysis", "前五大客户利润分析", "ai_report", "", "top_x_customer_profit_analysis_print"),

    TOP_X_SUPPLIER_PURCHASE_ANALYSIS_PRINT("top_x_supplier_purchase_analysis_analysis", "前五大供应商采购分析", "ai_report", "", "top_x_supplier_purchase_analysis_print"),

    MANAGEMENT_ACCOUNTING_PROFIT_LOSS_STATEMENT_PRINT("management_accounting_profit_loss_statement_analysis", "管理会计损益表", "ai_report", "", "management_accounting_profit_loss_statement_print"),

    PROFIT_LOSS_BALANCE_ANALYSIS_REPORT_PRINT("profit_loss_balance_analysis_report", "盈亏平衡分析报告", "ai_report", "", "profit_loss_balance_analysis_report_print"),

    // 数据查询类意图
    CUSTOMER_ACCOUNTS_RECEIVABLE_BALANCE_QUERY("accounts_receivable_query", "应收查询", "data_query", "customer_name", "accounts_receivable_query"),
    CUSTOMER_CUSTOMER_CODE_QUERY("customer_customer_code_query", "客户编码查询", "data_query", "customer_name", "accounts_receivable_query", List.of("客户编码", "客户名")),

    CUSTOMER_PROFIT_ANALYSIS_QUERY("customer_profit_analysis_query", "客户获利查询", "data_query", "customer_name", "customer_profit_analysis_query"),
    CUSTOMER_GROSS_PROFIT_QUERY("customer_gross_profit_query", "客户毛利查询", "data_query", "customer_name", "customer_profit_analysis_query", List.of("毛利", "客户名")),
    CUSTOMER_GROSS_PROFIT_RATE_QUERY("customer_gross_profit_rate_query", "客户毛利率率查询", "data_query", "customer_name", "customer_profit_analysis_query", List.of("毛利率", "客户名")),
    CUSTOMER_SHIPMENT_INCOME_QUERY("customer_shipment_income_query", "客户出货收入查询", "data_query", "customer_name", "customer_profit_analysis_query", List.of("出货收入", "客户名")),
    CUSTOMER_SHIPMENT_MATERIAL_COST_QUERY("customer_shipment_material_cost_query", "客户出货材料成本查询", "data_query", "customer_name", "customer_profit_analysis_query", List.of("出货材料成本", "客户名")),

    INVENTORY_QUERY("inventory_query", "库存查询", "data_query", "product", "inventory_query"),


    CUSTOMER_SALES_REPORT_QUERY("customer_sales_report_query", "客户销售报表查询", "data_query", "customer_name", "customer_sales_report_query"),

    EMPLOYEE_SALES_REPORT_QUERY("employee_sales_report_query", "员工销售报表查询", "data_query", "employee_name", "employee_sales_report_query"),

    DAYS_OBSOLETE_INVENTORY_QUERY_30("30_days_obsolete_inventory_query", "30天久滞库存查询", "data_query", "x_days", "30_days_obsolete_inventory_query"),
    DAYS_OBSOLETE_INVENTORY_QUERY_60("60_days_obsolete_inventory_query", "60天久滞库存查询", "data_query", "x_days", "60_days_obsolete_inventory_query"),
    DAYS_OBSOLETE_INVENTORY_QUERY_90("90_days_obsolete_inventory_query", "90天久滞库存查询", "data_query", "x_days", "90_days_obsolete_inventory_query"),

    EMPLOYEE_EXPENSES_QUERY("employee_expenses_query", "员工费用查询", "data_query", "employee_name", "employee_expenses_query"),

    DEPARTMENT_EXPENSES_QUERY("department_expenses_query", "部门费用查询", "data_query", "department_name", "department_expenses_query"),

    ACCOUNTS_PAYABLE_QUERY("accounts_payable_query", "应付查询", "data_query", "supplier_name", "accounts_payable_query"),

    ACCOUNTS_RECEIVABLE_QUERY("accounts_receivable_query", "应收查询", "data_query", "customer_name", "accounts_receivable_query"),

    SUPPLIER_ACCOUNTS_PAYABLE_BALANCE_QUERY("supplier_accounts_payable_balance_query", "供应商应付余额查询", "data_query", "supplier_name", "accounts_payable_query", List.of("供应商名", "应付账款余额（收发货为基准的）")),

    SUPPLIER_SUPPLIER_CODE_QUERY("supplier_supplier_code_query", "供应商编码查询", "data_query", "supplier_name", "accounts_payable_query", List.of("供应商名", "供应商编码")),

    LATEST_BOM_COST_QUERY("latest_bom_cost_query", "最新bom成本查询", "data_query", "product", "latest_bom_cost_query"),

    LATEST_PURCHASE_QUERY("latest_purchase_query", "最新采购查询", "data_query", "product", "latest_purchase_query"),
    PRODUCT_SUPPLIER_QUERY("product_supplier_query", "产品供应商查询", "data_query", "product", "latest_purchase_query", List.of("供应商", "商品")),

    LAST_SALE_PRICE_QUERY("last_sale_price_query", "最新销售价格查询", "data_query", "product", "last_sale_price_query"),

    // 功能类意图
    GOODBYE("goodbye", "再见", "function", "", "GOODBYE"),

    GREET("greet", "打招呼", "function", "", "GREET"),

    LOAN("loan", "借款", "function", "", "LOAN_BILL"),

    MATERIAL_REQUISITION("material_requisition", "领料", "function", "", "MATERIAL_REQUISITION"),

    OTHER_GET("other_get", "其他收入单", "function", "", "OTHER_INCOME"),

    PAYMENT_APPLICATION("payment_application", "付款申请", "function", "", "PAYMENT_APPLICATION"),

    RECEIVE_APPLICATION("receive_application", "收款申请", "function", "", "RECEIPT"),

    REIMBURSEMENT("reimbursement", "报销", "function", "", "REIMBURSEMENT"),

    // 其他意图
    DEPARTMENT_EMPLOYEE_COUNT_QUERY("department_employee_count_query", "部门员工数量查询", "data_query", "department_name", "department_employee_count_query"),

    EMPLOYEE_EMAIL_QUERY("employee_email_query", "员工邮箱查询", "data_query", "employee_name", "employee_email_query"),

    EMPLOYEE_INFO_QUERY("employee_info_query", "员工信息查询", "data_query", "employee_name", "employee_info_query"),

    EMPLOYEE_PHONE_NUMBER_QUERY("employee_phone_number_query", "员工电话查询", "data_query", "employee_name", "employee_phone_number_query"),

    COMPANY_TOTAL_EMPLOYEE_COUNT_QUERY("company_total_employee_count_query", "公司总员工数量查询", "data_query", "", "company_total_employee_count_query"),
    ;

```

