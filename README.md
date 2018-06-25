Testlink usado na versão atual.

Before being added to Git, the following changes were made:


Latest Changes:


File: //testlinkti.stara.com.br/gui/templates/attachments_simple.inc.tpl

Before changes:

<div  style="text-align:left;margin:3px;background:#CDE;padding: 3px 3px 3px 3px;border-style: groove;border-width: thin;">
      <label for="uploadedFile_[{$attach_id}]" class="labelHolder">{$labels.local_file} </label>
      <img class="clickable" src="{$tlImages.activity}" title="{$labels.max_size_file_upload}: {$gui->import_limit} Bytes)">
      <input type="file" name="uploadedFile[{$attach_id}][]" id="uploadedFile_{$attach_id}" multiple 
               size="{#UPLOAD_FILENAME_SIZE#}" />
        &nbsp;&nbsp;&nbsp;&nbsp;
</div>




After the changes:

<div  style="text-align:left;margin:3px;background:#CDE;padding: 3px 3px 3px 3px;border-style: groove;border-width: thin;">
	<a href="javascript:openFileUploadWindow({$tc_old_exec.execution_id},'executions')">
      	&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<img src="http://testlinkti.stara.com.br/gui/themes/default/images/upload_s.png" title="Anexos" alt="Anexos" style="border:none"></a>
        Anexar arquivos
        &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</div>



icon added in:

//testlinkti.stara.com.br/gui/themes/default/images

upload_s.png



