# manual create all module dirs w.o. modman

---- create all dirs ------------

mkdir BPMedia_GDPR;
cd BPMedia_GDPR;
mkdir -p app/code/community/BPMedia/GDPR;
mkdir -p app/design/frontend/base/default/template/bpmedia;
mkdir -p app/design/frontend/base/default/layout/bpmedia;
mkdir -p app/locale/en_US/template/email/bpmedia/gdpr;
mkdir -p skin/frontend/base/default/css/bpmedia/gdpr;
mkdir -p app/etc/modules;

---- copy all code to created dirs ----------

cp -r ../src/BPMedia/GDPR/* app/code/community/BPMedia/GDPR/;
cp -r ../src/template/bpmedia/* app/design/frontend/base/default/template/bpmedia/;
cp -r ../src/layout/bpmedia/* app/design/frontend/base/default/layout/bpmedia/;
cp -r ../src/email/bpmedia/gdpr/* app/locale/en_US/template/email/bpmedia/gdpr/;
cp -r ../src/cookiealert.css skin/frontend/base/default/css/bpmedia/gdpr/cookiealert.css;
cp -r ../src/BPMedia_GDPR.xml app/etc/modules/;
