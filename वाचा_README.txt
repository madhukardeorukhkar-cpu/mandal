देवरुखकर मंडळ ॲप — मोबाईल Home Screen आयकॉन (प्रवेश-पान)
=========================================================

यामुळे काय मिळते:
 • मोबाईलवर मंडळाच्या लोगोचा स्वतःचा आयकॉन
 • उघडताना मरून splash, वर URL पट्टी नाही — पूर्ण स्क्रीन ॲपसारखे
 • ॲप तेच (Google Apps Script), फक्त त्याचे "दार" सुंदर

एकदाच करायचे (10 मिनिटे, मोफत — GitHub Pages):
 1. ॲपची लिंक मिळवा: ॲप → More → Upgrade System → (किंवा Apps Script → Deploy → Manage deployments) — /exec ने संपणारी लिंक.
 2. index.html उघडा आणि  const APP_URL = "PASTE_YOUR_EXEC_URL_HERE";  मध्ये ती लिंक paste करा.
 3. github.com वर खाते बनवा → New repository → नाव उदा. devrukhkar-mandal → Public.
 4. "Add file → Upload files" ने या फोल्डरमधील सर्व फाइल्स (index.html, manifest.webmanifest, sw.js, icon-192.png, icon-512.png) upload करा.
 5. Settings → Pages → Branch: main → Save. 1-2 मिनिटांत लिंक मिळेल: https://<तुमचे-नाव>.github.io/devrukhkar-mandal/
 6. ही नवीन लिंक भावकीला पाठवा. Chrome मध्ये उघडून ⋮ → "Add to Home screen / Install app".

टीप:
 • ॲपमध्ये बदल (Upgrade) केले तरी हे प्रवेश-पान पुन्हा बदलावे लागत नाही.
 • Deployment नवीन बनवला (लिंक बदलली) तरच APP_URL बदला.
 • पहिल्यांदा या नव्या लिंकवरून उघडताना एकदा Login करावे लागेल.


---------------------------------------------------------
नवीन (Install popup) — GitHub वर अपडेट कसे करायचे:
 1. GitHub वर आपल्या mandal repository मधील सध्याचे index.html उघडा आणि APP_URL ची लिंक Copy करून ठेवा.
 2. "Add file → Upload files" ने या ZIP मधील index.html, manifest.webmanifest आणि sw.js पुन्हा upload करा (जुने बदलले जातील) → Commit.
 3. नवीन index.html उघडा → ✏️ → APP_URL मध्ये तीच लिंक पुन्हा paste करा → Commit.
 4. 1-2 मिनिटांनी लिंक उघडल्यावर खाली "📲 देवरुखकर मंडळ ॲप Install करा" असा popup येईल.
