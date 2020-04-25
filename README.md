CreationCallback<List<TemplateDescriptor>> getTemplatesCreationCallback = new CreationCallback<List<TemplateDescriptor>>()
  {
      @Override
      public Context getContext()
      {
          …
      }

      @Override
      public void onCancel()
      {
          …
      }

      @Override
      public void onFailure(ProtectionException e)
      {
          …
      }

      @Override
      public void onSuccess(List<TemplateDescriptor> templateDescriptors)
      {
         …
      }
  };
  try
  {
          …
      mIAsyncControl = TemplateDescriptor.getTemplates(emailId, mRmsAuthCallback, getTemplatesCreationCallback);
  }
  catch (com.microsoft.rightsmanagement.exceptions.InvalidParameterException e)
  {
          …
  }

