# date pick
```
        <div class="d-flex flex-column mb-8">
		    <label class="fs-6 fw-semibold mb-2">Contract End Date * dd month yyyy</label>
            <div class="input-group flatpickr" >
                <input id="contract_end_date" value="<?php echo ($contract_end_date ? date('d M Y', strtotime($contract_end_date)) : null) ?>" class="form-control datepicker" data-input />
                <span class="input-group-text btn btn-default" title="clear" data-clear>clear</span>
            </div>
        </div>

<script src="<?php echo prefix_url;?>assets/plugins/global/plugins.bundle.js"></script>
<script type="text/javascript">
$(".flatpickr").flatpickr({
    enableTime: false,
    dateFormat: "d M Y",
    position: "above",
    wrap: true
});
</script>
```
