# Class CheckStatus

class checkStatus {
    # Contructor Class
    constructor(element, status){
    # add a new property to a constructor
        this.element = element
        this.status = status
    }

    checkStatusActive() {
        # This creates a constant with the name 'getElement', which has a value of this.element */
        const getElement = document.querySelectorAll(this.element)
        
        # Logic to check status
        if(this.status !== null || '') {
            getElement.innerHTML = 
            <div class="py-1 px-3 bg-green-500 rounded-xl text-white text-xm font-medium">
            Active
            </div>
        }else {
            getElement.innerHTML = 
            <div class="py-1 px-3 bg-green-500 rounded-xl text-white text-xm font-medium">
            InActive
            </div>
        }
    }
}
