# Comparing `tmp/pretix-mpesa-mz-1.0.2.tar.gz` & `tmp/pretix-mpesa-mz-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretix-mpesa-mz-1.0.2.tar", last modified: Fri May  5 17:11:22 2023, max compression
+gzip compressed data, was "pretix-mpesa-mz-1.1.0.tar", last modified: Thu May 11 15:04:08 2023, max compression
```

## Comparing `pretix-mpesa-mz-1.0.2.tar` & `pretix-mpesa-mz-1.1.0.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 17:11:22.584766 pretix-mpesa-mz-1.0.2/
--rw-rw-rw-   0        0        0      567 2023-04-26 15:46:37.000000 pretix-mpesa-mz-1.0.2/LICENSE
--rw-rw-rw-   0        0        0      173 2023-04-26 15:46:37.000000 pretix-mpesa-mz-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1686 2023-05-05 17:11:22.585764 pretix-mpesa-mz-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1391 2023-04-26 15:46:37.000000 pretix-mpesa-mz-1.0.2/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-05 17:11:22.484674 pretix-mpesa-mz-1.0.2/pretix_mpesa_mz.egg-info/
--rw-rw-rw-   0        0        0     1686 2023-05-05 17:11:21.000000 pretix-mpesa-mz-1.0.2/pretix_mpesa_mz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1007 2023-05-05 17:11:22.000000 pretix-mpesa-mz-1.0.2/pretix_mpesa_mz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 17:11:21.000000 pretix-mpesa-mz-1.0.2/pretix_mpesa_mz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-05-05 17:11:21.000000 pretix-mpesa-mz-1.0.2/pretix_mpesa_mz.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       15 2023-05-05 17:11:21.000000 pretix-mpesa-mz-1.0.2/pretix_mpesa_mz.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-05 17:11:22.508670 pretix-mpesa-mz-1.0.2/pretix_mpesamz/
--rw-rw-rw-   0        0        0       23 2023-05-05 17:08:46.000000 pretix-mpesa-mz-1.0.2/pretix_mpesamz/__init__.py
--rw-rw-rw-   0        0        0      753 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.0.2/pretix_mpesamz/apps.py
-drwxrwxrwx   0        0        0        0 2023-05-05 17:11:22.422666 pretix-mpesa-mz-1.0.2/pretix_mpesamz/locale/
-drwxrwxrwx   0        0        0        0 2023-05-05 17:11:22.420665 pretix-mpesa-mz-1.0.2/pretix_mpesamz/locale/de/
-drwxrwxrwx   0        0        0        0 2023-05-05 17:11:22.519626 pretix-mpesa-mz-1.0.2/pretix_mpesamz/locale/de/LC_MESSAGES/
--rw-rw-rw-   0        0        0      308 2023-05-03 17:00:39.000000 pretix-mpesa-mz-1.0.2/pretix_mpesamz/locale/de/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0      321 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.0.2/pretix_mpesamz/locale/de/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-05-05 17:11:22.524628 pretix-mpesa-mz-1.0.2/pretix_mpesamz/locale/de_Informal/
--rw-rw-rw-   0        0        0        0 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.0.2/pretix_mpesamz/locale/de_Informal/.gitkeep
-drwxrwxrwx   0        0        0        0 2023-05-05 17:11:22.533792 pretix-mpesa-mz-1.0.2/pretix_mpesamz/locale/de_Informal/LC_MESSAGES/
--rw-rw-rw-   0        0        0      308 2023-05-03 17:00:39.000000 pretix-mpesa-mz-1.0.2/pretix_mpesamz/locale/de_Informal/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0      321 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.0.2/pretix_mpesamz/locale/de_Informal/LC_MESSAGES/django.po
--rw-rw-rw-   0        0        0     8589 2023-05-05 17:09:40.000000 pretix-mpesa-mz-1.0.2/pretix_mpesamz/payment.py
--rw-rw-rw-   0        0        0      352 2023-04-28 14:11:38.000000 pretix-mpesa-mz-1.0.2/pretix_mpesamz/signals.py
-drwxrwxrwx   0        0        0        0 2023-05-05 17:11:22.427666 pretix-mpesa-mz-1.0.2/pretix_mpesamz/static/
-drwxrwxrwx   0        0        0        0 2023-05-05 17:11:22.540773 pretix-mpesa-mz-1.0.2/pretix_mpesamz/static/pretix_mpesamz/
--rw-rw-rw-   0        0        0        0 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.0.2/pretix_mpesamz/static/pretix_mpesamz/.gitkeep
-drwxrwxrwx   0        0        0        0 2023-05-05 17:11:22.429666 pretix-mpesa-mz-1.0.2/pretix_mpesamz/templates/
-drwxrwxrwx   0        0        0        0 2023-05-05 17:11:22.573764 pretix-mpesa-mz-1.0.2/pretix_mpesamz/templates/pretix_mpesamz/
--rw-rw-rw-   0        0        0        0 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.0.2/pretix_mpesamz/templates/pretix_mpesamz/.gitkeep
--rw-rw-rw-   0        0        0      346 2023-04-26 15:53:24.000000 pretix-mpesa-mz-1.0.2/pretix_mpesamz/templates/pretix_mpesamz/checkout_payment_confirm.html
--rw-rw-rw-   0        0        0     4010 2023-05-03 14:29:30.000000 pretix-mpesa-mz-1.0.2/pretix_mpesamz/templates/pretix_mpesamz/checkout_payment_form.html
--rw-rw-rw-   0        0        0      280 2023-05-03 13:51:46.000000 pretix-mpesa-mz-1.0.2/pretix_mpesamz/templates/pretix_mpesamz/control.html
--rw-rw-rw-   0        0        0      184 2023-04-27 15:38:33.000000 pretix-mpesa-mz-1.0.2/pretix_mpesamz/templates/pretix_mpesamz/order.html
--rw-rw-rw-   0        0        0     1075 2023-04-26 15:54:54.000000 pretix-mpesa-mz-1.0.2/pretix_mpesamz/templates/pretix_mpesamz/redirect.html
--rw-rw-rw-   0        0        0      903 2023-05-05 17:11:22.587768 pretix-mpesa-mz-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1142 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-05 17:11:22.579764 pretix-mpesa-mz-1.0.2/tests/
--rw-rw-rw-   0        0        0       75 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.0.2/tests/test_main.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:04:08.626879 pretix-mpesa-mz-1.1.0/
+-rw-rw-rw-   0        0        0      567 2023-04-26 15:46:37.000000 pretix-mpesa-mz-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0      173 2023-04-26 15:46:37.000000 pretix-mpesa-mz-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1686 2023-05-11 15:04:08.627883 pretix-mpesa-mz-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1391 2023-04-26 15:46:37.000000 pretix-mpesa-mz-1.1.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-11 15:04:08.444893 pretix-mpesa-mz-1.1.0/pretix_mpesa_mz.egg-info/
+-rw-rw-rw-   0        0        0     1686 2023-05-11 15:04:07.000000 pretix-mpesa-mz-1.1.0/pretix_mpesa_mz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1068 2023-05-11 15:04:08.000000 pretix-mpesa-mz-1.1.0/pretix_mpesa_mz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 15:04:07.000000 pretix-mpesa-mz-1.1.0/pretix_mpesa_mz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-05-11 15:04:07.000000 pretix-mpesa-mz-1.1.0/pretix_mpesa_mz.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       15 2023-05-11 15:04:07.000000 pretix-mpesa-mz-1.1.0/pretix_mpesa_mz.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-11 15:04:08.487881 pretix-mpesa-mz-1.1.0/pretix_mpesamz/
+-rw-rw-rw-   0        0        0       23 2023-05-11 15:01:48.000000 pretix-mpesa-mz-1.1.0/pretix_mpesamz/__init__.py
+-rw-rw-rw-   0        0        0      753 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.1.0/pretix_mpesamz/apps.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:04:08.361879 pretix-mpesa-mz-1.1.0/pretix_mpesamz/locale/
+drwxrwxrwx   0        0        0        0 2023-05-11 15:04:08.359879 pretix-mpesa-mz-1.1.0/pretix_mpesamz/locale/de/
+drwxrwxrwx   0        0        0        0 2023-05-11 15:04:08.506914 pretix-mpesa-mz-1.1.0/pretix_mpesamz/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0        0        0      308 2023-05-03 17:00:39.000000 pretix-mpesa-mz-1.1.0/pretix_mpesamz/locale/de/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0      321 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.1.0/pretix_mpesamz/locale/de/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2023-05-11 15:04:08.519884 pretix-mpesa-mz-1.1.0/pretix_mpesamz/locale/de_Informal/
+-rw-rw-rw-   0        0        0        0 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.1.0/pretix_mpesamz/locale/de_Informal/.gitkeep
+drwxrwxrwx   0        0        0        0 2023-05-11 15:04:08.540881 pretix-mpesa-mz-1.1.0/pretix_mpesamz/locale/de_Informal/LC_MESSAGES/
+-rw-rw-rw-   0        0        0      308 2023-05-03 17:00:39.000000 pretix-mpesa-mz-1.1.0/pretix_mpesamz/locale/de_Informal/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0      321 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.1.0/pretix_mpesamz/locale/de_Informal/LC_MESSAGES/django.po
+-rw-rw-rw-   0        0        0    11909 2023-05-11 14:52:54.000000 pretix-mpesa-mz-1.1.0/pretix_mpesamz/payment.py
+-rw-rw-rw-   0        0        0      352 2023-04-28 14:11:38.000000 pretix-mpesa-mz-1.1.0/pretix_mpesamz/signals.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:04:08.367877 pretix-mpesa-mz-1.1.0/pretix_mpesamz/static/
+drwxrwxrwx   0        0        0        0 2023-05-11 15:04:08.550880 pretix-mpesa-mz-1.1.0/pretix_mpesamz/static/pretix_mpesamz/
+-rw-rw-rw-   0        0        0        0 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.1.0/pretix_mpesamz/static/pretix_mpesamz/.gitkeep
+drwxrwxrwx   0        0        0        0 2023-05-11 15:04:08.372883 pretix-mpesa-mz-1.1.0/pretix_mpesamz/templates/
+drwxrwxrwx   0        0        0        0 2023-05-11 15:04:08.612882 pretix-mpesa-mz-1.1.0/pretix_mpesamz/templates/pretix_mpesamz/
+-rw-rw-rw-   0        0        0        0 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.1.0/pretix_mpesamz/templates/pretix_mpesamz/.gitkeep
+-rw-rw-rw-   0        0        0      346 2023-04-26 15:53:24.000000 pretix-mpesa-mz-1.1.0/pretix_mpesamz/templates/pretix_mpesamz/checkout_payment_confirm.html
+-rw-rw-rw-   0        0        0     4010 2023-05-03 14:29:30.000000 pretix-mpesa-mz-1.1.0/pretix_mpesamz/templates/pretix_mpesamz/checkout_payment_form.html
+-rw-rw-rw-   0        0        0      380 2023-05-11 14:14:56.000000 pretix-mpesa-mz-1.1.0/pretix_mpesamz/templates/pretix_mpesamz/control.html
+-rw-rw-rw-   0        0        0      236 2023-05-11 14:34:44.000000 pretix-mpesa-mz-1.1.0/pretix_mpesamz/templates/pretix_mpesamz/order.html
+-rw-rw-rw-   0        0        0      452 2023-05-11 14:57:44.000000 pretix-mpesa-mz-1.1.0/pretix_mpesamz/templates/pretix_mpesamz/payment_pending.html
+-rw-rw-rw-   0        0        0     1075 2023-04-26 15:54:54.000000 pretix-mpesa-mz-1.1.0/pretix_mpesamz/templates/pretix_mpesamz/redirect.html
+-rw-rw-rw-   0        0        0      903 2023-05-11 15:04:08.630881 pretix-mpesa-mz-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1142 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:04:08.619879 pretix-mpesa-mz-1.1.0/tests/
+-rw-rw-rw-   0        0        0       75 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.1.0/tests/test_main.py
```

### Comparing `pretix-mpesa-mz-1.0.2/LICENSE` & `pretix-mpesa-mz-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pretix-mpesa-mz-1.0.2/PKG-INFO` & `pretix-mpesa-mz-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretix-mpesa-mz
-Version: 1.0.2
+Version: 1.1.0
 Summary: A plugin to allow payments through the M-Pesa mobile payment platform
 Home-page: https://github.com/ivanruby/pretix-mpesa-mz
 Author: Ivan Ruby
 Author-email: ivanrubyds@gmail.com
 License: Apache
 License-File: LICENSE
```

### Comparing `pretix-mpesa-mz-1.0.2/README.rst` & `pretix-mpesa-mz-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `pretix-mpesa-mz-1.0.2/pretix_mpesa_mz.egg-info/PKG-INFO` & `pretix-mpesa-mz-1.1.0/pretix_mpesa_mz.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretix-mpesa-mz
-Version: 1.0.2
+Version: 1.1.0
 Summary: A plugin to allow payments through the M-Pesa mobile payment platform
 Home-page: https://github.com/ivanruby/pretix-mpesa-mz
 Author: Ivan Ruby
 Author-email: ivanrubyds@gmail.com
 License: Apache
 License-File: LICENSE
```

### Comparing `pretix-mpesa-mz-1.0.2/pretix_mpesa_mz.egg-info/SOURCES.txt` & `pretix-mpesa-mz-1.1.0/pretix_mpesa_mz.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -19,9 +19,10 @@
 pretix_mpesamz/locale/de_Informal/LC_MESSAGES/django.po
 pretix_mpesamz/static/pretix_mpesamz/.gitkeep
 pretix_mpesamz/templates/pretix_mpesamz/.gitkeep
 pretix_mpesamz/templates/pretix_mpesamz/checkout_payment_confirm.html
 pretix_mpesamz/templates/pretix_mpesamz/checkout_payment_form.html
 pretix_mpesamz/templates/pretix_mpesamz/control.html
 pretix_mpesamz/templates/pretix_mpesamz/order.html
+pretix_mpesamz/templates/pretix_mpesamz/payment_pending.html
 pretix_mpesamz/templates/pretix_mpesamz/redirect.html
 tests/test_main.py
```

### Comparing `pretix-mpesa-mz-1.0.2/pretix_mpesamz/apps.py` & `pretix-mpesa-mz-1.1.0/pretix_mpesamz/apps.py`

 * *Files identical despite different names*

### Comparing `pretix-mpesa-mz-1.0.2/pretix_mpesamz/payment.py` & `pretix-mpesa-mz-1.1.0/pretix_mpesamz/payment.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,32 +10,33 @@
 from django.utils.translation import ugettext_lazy as _
 from django.template.loader import get_template
 from django import forms
 
 from paymentsds.mpesa import Client
 from random import randint
 
+
 class MpesaPayment(BasePaymentProvider):
     identifier = 'mpesa'
 
     ########################################################
     #                   General Settings
     ########################################################
     @property
     def verbose_name(self):
         return str(self.settings.get('method_name', as_type=LazyI18nString) or _('M-Pesa'))
 
     @property
     def confirm_button_name(self):
         return _('Pagar via M-Pesa')
-    
+
     @property
     def priority(self):
         return 100
-    
+
     ########################################################
     #                Control Panel Settings
     ########################################################
     @property
     def information_text(self):
         return rich_text(self.settings.get('information_text', as_type=LazyI18nString))
 
@@ -46,128 +47,133 @@
     @property
     def payment_completed_text(self):
         return rich_text(self.settings.get('payment_completed_text', as_type=LazyI18nString))
 
     @property
     def settings_form_fields(self):
         service_provider_code_field = forms.CharField(
-            label = _('Código de Provedor de Serviço M-Pesa'),
+            label=_('Código de Provedor de Serviço M-Pesa'),
             help_text=_('Identificador da entidade fornecido pelo M-Pesa')
         )
 
         api_key_field = forms.CharField(
-            label = _('API Key'),
+            label=_('API Key'),
             help_text=_('API Key fornecido pelo M-Pesa')
         )
 
         public_key_field = forms.CharField(
-            label = _('Public Key'),
+            label=_('Public Key'),
             help_text=_('Public Key fornecido pelo M-Pesa')
         )
 
         info_field = I18nFormField(
-            label = _('Payment information text'),
+            label=_('Payment information text'),
             help_text=_('Shown to the user when selecting a payment method.'),
-            widget = I18nTextarea,
+            widget=I18nTextarea,
         )
         pending_field = I18nFormField(
-            label = _('Payment pending text'),
-            help_text = _('Shown to the user when viewing a pending payment order.'),
-            widget = I18nTextarea,
+            label=_('Payment pending text'),
+            help_text=_(
+                'Shown to the user when viewing a pending payment order.'),
+            widget=I18nTextarea,
         )
         completed_field = I18nFormField(
-            label = _('Payment completed text'),
-            help_text = _('Shown to the user when viewing an order with completed payment.'),
-            widget = I18nTextarea,
+            label=_('Payment completed text'),
+            help_text=_(
+                'Shown to the user when viewing an order with completed payment.'),
+            widget=I18nTextarea,
         )
 
         settingsList = [
-                ('service_provider_code', service_provider_code_field),
-                ('api_key', api_key_field),
-                ('public_key', public_key_field),
-                ('information_text', info_field),
-                ('payment_pending_text', pending_field),
-                ('payment_completed_text', completed_field)
+            ('service_provider_code', service_provider_code_field),
+            ('api_key', api_key_field),
+            ('public_key', public_key_field),
+            ('information_text', info_field),
+            ('payment_pending_text', pending_field),
+            ('payment_completed_text', completed_field)
         ]
 
         return OrderedDict(list(super().settings_form_fields.items()) + settingsList)
 
     ########################################################
     #               Checkout process settings
     ########################################################
     def payment_is_valid_session(self, request):
         return all([
-            request.session.get('payment_%s_msisdn' % self.identifier, '') != ''
+            request.session.get('payment_%s_msisdn' %
+                                self.identifier, '') != ''
         ])
-    
+
     def order_change_allowed(self, order):
         return True
 
-    
     ########################################################
     #                   General Settings
     ########################################################
+
     @property
     def payment_form_fields(self):
         # Validate: ensure only valid numbers can be entered
         msisdn_field = ('msisdn',
-            forms.IntegerField(
-            label='Número (+258):',
-            required=True,
-            min_value=840000000,
-            max_value=859999999,
-            error_messages={'invalid':'Por favor, introduza um número 84 ou 85 válido'}
-        ))
+                        forms.IntegerField(
+                            label='Número (+258):',
+                            required=True,
+                            min_value=840000000,
+                            max_value=859999999,
+                            error_messages={
+                                'invalid': 'Por favor, introduza um número 84 ou 85 válido'}
+                        ))
         return OrderedDict([
             msisdn_field,
         ])
-    
+
     def payment_form_render(self, request):
         form = self.payment_form(request)
         template = get_template('pretix_mpesamz/checkout_payment_form.html')
         ctx = {
-                'request': request, 
-                'form': form,
-                'information_text': self.information_text,
+            'request': request,
+            'form': form,
+            'information_text': self.information_text,
         }
         return template.render(ctx)
-    
+
     def checkout_confirm_render(self, request):
         template = get_template('pretix_mpesamz/order.html')
         ctx = {
             'information_text': self.information_text,
             'msisdn': request.session.get('payment_%s_msisdn' % self.identifier)
         }
         return template.render(ctx)
 
     def execute_mpesa_payment(self, payload):
         client = Client(
-            api_key = self.settings.get('api_key'),          
+            api_key=self.settings.get('api_key'),
             public_key=self.settings.get('public_key'),
             service_provider_code=self.settings.get('service_provider_code')
         )
-     
+
         return client.receive(payload)
 
-        
     def execute_payment(self, request, payment):
         msisdn = request.session.get('payment_%s_msisdn' % self.identifier, '')
 
         try:
             payment_data = {
-                'from': "258" + str(msisdn),   
-                'reference': payment.order.code,      
-                'transaction': 'TEST' + str(randint(0, 1000)), 
+                'from': "258" + str(msisdn),
+                'reference': payment.order.code,
+                'transaction': 'TEST' + str(randint(0, 1000)),
                 'amount': str(int(float(payment.amount)))
             }
 
             result = self.execute_mpesa_payment(payment_data)
+            print(vars(result))
 
             if result.success:
                 success_payload = json.dumps({
+                    'success': True,
                     'code': result.status.code,
                     'msisdn': msisdn,
                     'conversation': result.data['conversation'],
                     'description': result.status.description
                 })
                 # Displayed in control panel but not on API order response
                 payment.info = success_payload
@@ -175,28 +181,99 @@
                 # Add success payload to a field returned on Order Endpoint
                 payment.order.meta_info = success_payload
                 payment.order.save(update_fields=['meta_info'])
 
                 payment.save(update_fields=['info'])
                 payment.confirm()
             else:
+                error_payload = json.dumps({
+                    'success': False,
+                    'msisdn': msisdn,
+                    'code': result.status.code,
+                    'conversation': result.data['conversation'],
+                    'description': result.status.description
+                })
+
+                # Displayed in control panel but not on API order response
+                payment.info = error_payload
+
+                payment.save(update_fields=['info'])
                 payment.fail()
-            
-            return 
+
+            return
         except Exception as e:
             print(repr(e))
-    
+
+    def payment_prepare(self, request, payment):
+        msisdn = request.session.get(
+            'payment_%s_msisdn' % self.identifier, '')
+
+        try:
+            payment_data = {
+                'from': "258" + str(msisdn),
+                'reference': payment.order.code + str(randint(0, 10)),
+                'transaction': 'TEST' + str(randint(0, 1000)),
+                'amount': str(int(float(payment.amount)))
+            }
+
+            result = self.execute_mpesa_payment(payment_data)
+            print(vars(result))
+
+            if result.success:
+                success_payload = json.dumps({
+                    'success': True,
+                    'code': result.status.code,
+                    'msisdn': msisdn,
+                    'conversation': result.data['conversation'],
+                    'description': result.status.description
+                })
+                # Displayed in control panel but not on API order response
+                payment.info = success_payload
+
+                # Add success payload to a field returned on Order Endpoint
+                payment.order.meta_info = success_payload
+                payment.order.save(update_fields=['meta_info'])
+
+                payment.save(update_fields=['info'])
+                payment.confirm()
+            else:
+                error_payload = json.dumps({
+                    'success': False,
+                    'msisdn': msisdn,
+                    'code': result.status.code,
+                    'conversation': result.data['conversation'],
+                    'description': result.status.description
+                })
+
+                # Displayed in control panel but not on API order response
+                payment.info = error_payload
+
+                payment.save(update_fields=['info'])
+                payment.fail()
+
+            return
+        except Exception as e:
+            print(repr(e))
+
     def payment_pending_render(self, request, payment) -> str:
-        template = get_template('pretix_mpesamz/order.html')
+        template = get_template('pretix_mpesamz/payment_pending.html')
         if payment.info:
             payment_info = json.loads(payment.info)
         else:
             return _("No payment information available.")
+
+        if payment_info['code'] == "INS-6":
+            reason = "PIN incorreto"
+        elif payment_info['code'] == "INS-9":
+            reason = "demora na comunicação entre a aplicação e o M-Pesa"
+        elif payment_info['code'] == "INS-10":
+            reason = "transação duplicada"
+
         ctx = {
-            'information_text': self.payment_pending_text,
+            'reason': reason,
             'msisdn': request.session.get('payment_%s_msisdn' % self.identifier, '')
         }
         return template.render(ctx)
 
     def order_completed_render(self, request, order) -> str:
         template = get_template('pretix_mpesamz/order.html')
         if order.payment_info:
@@ -206,24 +283,33 @@
         ctx = {
             'information_text': self.payment_completed_text,
             'msisdn': self.msisdn
         }
         return template.render(ctx)
 
     ########################################################
-    #                   Called to display Order 
+    #                   Called to display Order
     #                   info in Control Panel
     ########################################################
     def payment_control_render(self, request, payment) -> str:
         template = get_template('pretix_mpesamz/control.html')
 
-        if payment.info is not None or 'conversation' in payment.info:
+        if payment.info is not None and 'conversation' in payment.info:
             payment_info = json.loads(payment.info)
+            if payment_info['success']:
+                ctx = {
+                    'conversationID': payment_info['conversation'],
+                    'msisdn': payment_info['msisdn'],
+                    'description': payment_info['description'],
+                    'code': payment_info['code']
+                }
+            else:
+                ctx = {
+                    'conversationID': payment_info['conversation'],
+                    'msisdn': payment_info['msisdn'],
+                    'code': payment_info['code'],
+                    'description': payment_info['description'],
+                }
         else:
             return _("Pagamento via M-Pesa sem sucesso.")
-        
-        ctx = {
-            'conversationID': payment_info['conversation'],
-            'msisdn': payment_info['msisdn'],
-            'description': payment_info['description'],
-        }
-        return template.render(ctx)
+
+        return template.render(ctx)
```

### Comparing `pretix-mpesa-mz-1.0.2/pretix_mpesamz/templates/pretix_mpesamz/checkout_payment_form.html` & `pretix-mpesa-mz-1.1.0/pretix_mpesamz/templates/pretix_mpesamz/checkout_payment_form.html`

 * *Files identical despite different names*

### Comparing `pretix-mpesa-mz-1.0.2/pretix_mpesamz/templates/pretix_mpesamz/redirect.html` & `pretix-mpesa-mz-1.1.0/pretix_mpesamz/templates/pretix_mpesamz/redirect.html`

 * *Files identical despite different names*

### Comparing `pretix-mpesa-mz-1.0.2/setup.cfg` & `pretix-mpesa-mz-1.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pretix-mpesa-mz-1.0.2/setup.py` & `pretix-mpesa-mz-1.1.0/setup.py`

 * *Files identical despite different names*

