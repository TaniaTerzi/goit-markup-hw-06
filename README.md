# goit-markup-hw-06

<label class="modal-form-option-label"> 
            <input type="checkbox" name="policy" value="accept-policy" class="modal-form-checkbox">
            <span class="modal-form-custom-checkbox">
                <svg class="modal-form-checkbox-icon" width="11" height="8"> 
                    <use href="./images/sprite.svg#icon-check-icon"></use>
                </svg>
            </span>
            <span class="modal-form-option-span">I accept the terms and conditions of the <a class="modal-form-link" href="">Privacy Policy</a></span>
        </label>

а у стилях

.modal-form-checkbox {
  position: absolute;
  width: 1px;
  height: 1px;
  margin: -1px;
  border: 0;
  padding: 0;
  flex-shrink: 0;
  clip: rect(0 0 0 0);
  overflow: hidden;
  border-radius: 2px;
}


.modal-form-custom-checkbox {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  width: 16px;
  height: 15px;
  margin-left: 10px;
  margin-right: 10px;
  border: 2px solid var(--title-color);
}

.modal-form-checkbox-icon {
  display: block;
  align-items: center;
  justify-content: center;
  opacity: 0;
}

.modal-form-checkbox:checked + .modal-form-custom-checkbox {
  background-color: var(--accent-color);
  border: 1px solid var(--accent-color);
}

.modal-form-checkbox:checked + .modal-form-custom-checkbox .modal-form-checkbox-icon {
  opacity: 1;
  fill: var(--secondary-color);
}