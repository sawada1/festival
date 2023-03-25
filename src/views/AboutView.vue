<template>
  <section class="ticket-section section-padding">
                <div class="section-overlay"></div>

                <div class="container">
                    <div class="row">

                        <div class="col-lg-6 col-10 mx-auto">
                            <form class="custom-form ticket-form mb-5 mb-lg-0" action="#" method="post" role="form">
                                <h2 class="text-center mb-4">Get started here</h2>

                                <div class="ticket-form-body">
                                    <div class="row m-2">
                                        <div class="col-lg-6 col-md-6 col-12">
                                            <input type="text" name="ticket-form-name" id="ticket-form-name" class="form-control" placeholder="Full name" required>
                                        </div>

                                        <div class="col-lg-6 col-md-6 col-12">
                                            <input type="email" name="ticket-form-email" id="ticket-form-email" pattern="[^ @]*@[^ @]*" class="form-control" placeholder="Email address" required>
                                        </div>
                                    </div>

                                    <input type="tel" class="form-control my-3" name="ticket-form-phone" placeholder="Ph 01021189596" pattern="[0-9]{3}-[0-9]{3}-[0-9]{4}" required>

                                    <h6>Choose Ticket Type</h6>

                                    <div class="row my-3">
                                        <div class="col-lg-6 col-md-6 col-12">
                                            <div class="form-check form-control">
                                                <input class="form-check-input" type="radio" name="TicketForm" id="flexRadioDefault1">
                                                <label class="form-check-label" for="flexRadioDefault1">
                                                    Eary bird $120
                                                </label>
                                            </div>
                                        </div>

                                        <div class="col-lg-6 col-md-6 col-12">
                                            <div class="form-check form-check-radio form-control">
                                                <input class="form-check-input" type="radio" name="TicketForm" id="flexRadioDefault2">
                                                <label class="form-check-label" for="flexRadioDefault2">
                                                    Standard $240
                                                </label>
                                            </div>
                                        </div>
                                    </div>

                                    <input type="number" name="ticket-form-number" id="ticket-form-number" class="form-control my-3" placeholder="Number of Tickets" required>

                                    <textarea name="ticket-form-message" rows="3" class="form-control" id="ticket-form-message" placeholder="Additional Request"></textarea>

                                    <div class="col-lg-4 col-md-10 col-8 mx-auto">
                                        <button type="submit" class=" btn btn-warning text-light p-3 fs-6 form-control my-3">Buy Ticket</button>
                                    </div>
                                </div>
                            </form>
                    </div>
                </div>
                </div>
            </section>
</template>



<style>

.ticket-section {
  background-image: url('../assets/images/nicholas-green-unsplash-blur.jpg');
  background-repeat: no-repeat;
  background-size: cover;
  position: relative;
  padding-top: 130px;
}

.ticket-form {
  background: #fff;
  border-radius: 20px;
  padding: 50px;
}

.ticket-form .form-check {
  position: relative;
  min-height: 52px;
  padding-left: 35px;
}

.ticket-form .form-check .form-check-label {
  display: block;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  margin-top: 12px;
  margin-left: 35px;
  width: 100%;
  height: 100%;
}

</style>
