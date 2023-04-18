# CTDropTarget : COleDropTarget
+ public:
  +   CHAR curdir[260]
  +   CHAR info[260]
  +   CString url
  +   CString titre
  +   CTDropTarget()
  +   virtual DROPEFFECT OnDragOver(CWnd* pWnd, COleDataObject* pDataObject, DWORD dwKeyState, CPoint point)
  +   virtual BOOL OnDrop(CWnd* pWnd, COleDataObject* pDataObject, DROPEFFECT dropEffect, CPoint point)
    
# CGitCloneApp : CWinApp
+ public:
	+ CGitCloneApp()
	+ virtual BOOL InitInstance()

# CGitCloneDlg : CDialog
+ public:
	+ CGitCloneDlg(CWnd* pParent = nullptr)
	+ int MsgBox(CHAR* lpszText, CHAR* lpszCaption, DWORD dwStyle, INT lpszIcon)
	+ CEdit	m_ctlEdURL
	+ CListBox	m_url
	+ void OnEnChangeEdit1()
	+ void OnLbnSelchangeList1()
	+ void Telecharger(char* GitLink, bool Automatique)
	+ void OnBnClickedAboutbox()
	+ void OnBnClickedOk()
	+ void OnBnClickedButton2()
	+ void OnBnClickedButton1()
	+ void OnClose()
	+ void OnBnClickedCancel()
+ protected:
	+ virtual void DoDataExchange(CDataExchange* pDX)
	+ HICON m_hIcon;
	+ virtual BOOL OnInitDialog()
	+ void OnSysCommand(UINT nID, LPARAM lParam)
	+ void OnPaint()
	+ HCURSOR OnQueryDragIcon()
	+ void OnDropFiles(HDROP hDropInfo)

# CAboutDlg : CDialog
+ public:
	+ CAboutDlg()
  + void OnActivate(UINT nState, CWnd* pWndOther, BOOL bMinimized)
+ protected:
	+ virtual void DoDataExchange(CDataExchange* pDX)

